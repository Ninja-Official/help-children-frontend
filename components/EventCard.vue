<template>
  <NuxtLink class="not-decorate" v-bind:to="'/events/'+ id">
    <div class="card">
      <img class="preview-img" src="https://vdnh.ru/%D0%90%D1%80%D0%BA%D0%B0_A.C._-8267.jpg">
      <div class="date-container flex-el">
        <img src="../static/icon-calendar.svg">
        <p class="date text"> {{ date }} </p>
      </div>
      <h2 class="text flex-el"> {{ name }} </h2>
      <div class="location-container flex-el">
        <img src="../static/icon-map-pin.svg">
        <p class="location text"> {{ location }} </p>
      </div>
      <ActionButton />
    </div>
  </NuxtLink>
</template>

<script>
  export default {
    props: {
      id: {
        type: Number,
        default: 0
      },
      name: {
        type: String,
        default: "Название события"
      },
      date: {
        type: String,
        default: "12 марта 2021"
      },
      location: {
        type: String,
        default: "ул. ВДНХ к12"
      }
    }
  }
</script>

<style lang="scss" scoped>

@import "../assets/constants.scss";

$card-left-margin: 15px;

.card {
  display: flex;
  width: 400px;
  height: 300px;
  border-radius: 15px;
  background-color: rgb(255, 255, 255);
  box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.25);
  margin: 30px;
  text-decoration: none;

  h2 {
    font-size: $font-size-2;
    margin-left: $card-left-margin;
  }
}

.date-container {
  display: flex;
  
  .date {
    font-size: $font-size-1;
    font: bold;    
    margin: 10px 10px 0px;
  }
}

.flex-el {
  margin-left: $card-left-margin;
}

.location-container {
  display: flex;
}

.preview-img {
  height: 150px;
  border-radius: 15px;
}

.card:hover {
  background-color: rgb(250, 250, 250);
}

.text {
  margin-bottom: 0px;
  color: $font-gray-color;
}

.not-decorate {
  text-decoration: none;
}

</style>