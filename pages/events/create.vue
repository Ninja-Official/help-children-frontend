<template>
  <div>
    <PageBase>
      <div class="card">
        <EventProgressBar />
        <form id="event-submit-form">
          <div id="page-first" class="page first">
            <EventFormInputField text="Название мероприятия" name="name" />
            <EventFormInputField text="Для кого" name="consumers" />
            <UploadImages @changed="handleImages"/>
            <input type="hidden" id="event-images" name="event-images" />
            <div class="buttons-container">
              <ActionButton id="btn-goto-2-1" buttonText="Продолжить"></ActionButton>
            </div>
          </div>
          <div id="page-second" class="page second">
            <EventFormTextArea text="Необходимые ресурсы для проведения" name="resources" />
            <EventFormTextArea text="Описание мероприятия" name="description" />
            <div class="buttons-container">
              <ActionButton id="btn-goto-1" buttonText="Вернутся назад"></ActionButton>
              <ActionButton id="btn-goto-3" buttonText="Продолжить"></ActionButton>
            </div>
          </div>
          <div id="page-third" class="page third">
            <EventFormInputField text="Место проведения" name="location" />
            <EventFormInputField text="Дата проведения" name="date" />
            <div class="buttons-container">
              <ActionButton id="btn-goto-2-2" buttonText="Вернутся назад"></ActionButton>
              <ActionButton id="finish-button" buttonText="Завершить"></ActionButton>
            </div>
          </div>
        </form>
      </div>
    </PageBase>
  </div>
</template>

<script>
  import UploadImages from "vue-upload-drop-images";
  import axios from "@nuxtjs/axios";

  export default {
    components: {
      UploadImages,
    },
    mounted () {
      console.log(this)
      init(this.$axios);
    },
    methods: {
      handleImages(files){
        console.log(files);
        userPictures = files;
      }
    }
  }

  let userPictures;

  function init(axios) {
    document.getElementById("btn-goto-1").onclick = () => goToPage(1);
    document.getElementById("btn-goto-2-1").onclick = () => goToPage(2);
    document.getElementById("btn-goto-2-2").onclick = () => goToPage(2);
    document.getElementById("btn-goto-3").onclick = () => goToPage(3);
    document.getElementById("finish-button").onclick = () => submitForm(axios);
    goToPage(1);
  }

  function submitForm(axios) {
    alert("Aboba");
    console.log("ABABABABAB");
    let formData = new FormData(document.getElementById("event-submit-form"));
    userPictures.forEach(element => {
      formData.append('userpic[]', element, element.name)
    });
    console.log(axios);
    axios({
      method: "post",
      url: "https://127.0.0.1:5000/amogus",
      data: formData,
      headers: { "Content-Type": "multipart/form-data" },
    })
    .then(function (response) {
      //handle success
      console.log(response);
    })
    .catch(function (response) {
      //handle error
      console.log(response);
    });
  }

  function goToPage(page) {
    switch (page) {
      case 1:
        document.getElementById("page-first").style.display = "flex";
        document.getElementById("page-second").style.display = "none";
        document.getElementById("page-third").style.display = "none";
        document.getElementById("point-2").classList.add("inactive");
        document.getElementById("point-3").classList.add("inactive");
        break;
      case 2:
        document.getElementById("page-first").style.display = "none";
        document.getElementById("page-second").style.display = "flex";
        document.getElementById("page-third").style.display = "none";
        document.getElementById("point-2").classList.add("active");
        document.getElementById("point-3").classList.remove("active");
        document.getElementById("point-2").classList.remove("inactive");
        document.getElementById("point-3").classList.add("inactive");
        break;
      case 3: 
        document.getElementById("page-first").style.display = "none";
        document.getElementById("page-second").style.display = "none";
        document.getElementById("page-third").style.display = "flex";
        document.getElementById("point-1").classList.add("active");
        document.getElementById("point-2").classList.add("active");
        document.getElementById("point-3").classList.add("active");
        document.getElementById("point-3").classList.remove("inactive");
        break;
    }
  }

</script>

<style lang="scss" scoped>

@import "../../assets/constants.scss";

.card {
  display: flex;
  justify-content: space-between;
  min-height: 400px;
  border-radius: $card-border-radius;
  background-color: rgb(255, 255, 255);
  box-shadow: $main-box-shadow;
  margin: 30px;
  text-decoration: none;
  overflow: hidden;
  padding: $card-padding;

  h2 {
    font-size: $font-size-2;
    color: $font-bold-color;
    font-weight: bold;
    margin-left: 6px;
  }
}

form {
  flex: 5;
  padding: 20px;
  padding-top: 50px;
}

.page { 
  display: flex;
  height: 100%;
  flex-direction: column;
  justify-content: space-between;
  gap: 25px;
}

#pageFirst {
  
}

#pageSecond {
  display: none;
}

#pageThird {
  display: none;
}

.buttons-container {
  display: flex;
  justify-content: space-between;
}

</style>