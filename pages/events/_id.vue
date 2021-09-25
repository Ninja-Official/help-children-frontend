<template>
  <PageBase>
    <div class="container">
      <div class="card">
        <h1 class="title img-text">Title</h1>
        <p class="img-text">Aasd</p>
        <img src="https://play-lh.googleusercontent.com/8ddL1kuoNUB5vUvgDVjYY3_6HwQcrg1K2fd_R8soD-e2QYj8fT9cfhfh3G0hnSruLKec">
      </div>
      <div class="info-cards-container">
        <div class="card info-container">
          <h3>Статус</h3>
          <p1>Абоба</p1>
          <h3>Участники</h3>
          <p1>Воспитанники</p1>
          <h3>Необходимое</h3>
          <p1>Волонтеры</p1>
        </div>
        <div class="card description-container">
          <h1>Описание</h1>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
            labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
            nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
            esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
            culpa qui officia deserunt mollit anim id est laborum.
          </p>
          <div class="buttons-container">
            <ActionButton class="apply-button" buttonText="Хочу сходить" />
            <ActionButton class="apply-button" buttonImage="../static/Vector.svg" />
          </div>
        </div>
      </div>
    </div>
  </PageBase>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>

@import "../../assets/constants.scss";

$card-padding: 30px;

h1 {
  
}

.apply-button {
  padding: 20px;
}

.chat-button {

}

.description-container {
  flex: 9;
}

.info-container {
  flex: 3;
  display: flex;
  flex-direction: column;
}

.info-cards-container {
  display: flex;
}

.buttons-container {
  display: flex;
  gap: 10px;
}

img {
  margin: -$card-padding;
  max-height:350px;
  object-fit:cover;
  object-position:50% 50%;
  overflow: hidden;
}

.container {
  display: flex;
  justify-content: center;
  flex-direction: column;
}

.card {
  margin: 15px;
  padding: $card-padding;
  box-shadow: $main-box-shadow;
  border-radius: 25px;
  overflow: hidden;

  .title {
    top: 20px;
    left: 20px;
  }

  .img-text {
    position: absolute;
    color: $font-bright-color;
  }
}

</style>