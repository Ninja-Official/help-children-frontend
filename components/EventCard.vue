<template>
  <NuxtLink class="not-decorate" v-bind:to="'/events/'+ id">
    <div class="card">
      <img class="preview-img" src="https://vdnh.ru/%D0%90%D1%80%D0%BA%D0%B0_A.C._-8267.jpg">
      <DateInfo class="text" v-bind:date="date"/>
      <h2 class="text"> {{ name }} </h2>
      <LocationInfo class="text" v-bind:location="location" />
      <ActionButton buttonText="Хочу пойти!" class="apply-button" />
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
$card-padding: 15px;

.card {
  display: flex;
  width: 400px;
  height: 400px;
  border-radius: 15px;
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

.date-container {
  display: flex; 
  align-items: center;

  .date {
    font-size: $font-size-1;
  }
}

.location-container {
  display: flex;
  font-weight: bold;
}

.apply-button {
  margin: 10px;
}

.preview-img {
  margin: -$card-padding;
  margin-bottom: 5px;
  height: 225px;
  object-fit:cover;
  object-position:50% 50%;
}

.card:hover {
  background-color: rgb(250, 250, 250);
}

.text {
  margin-bottom: 0px;
  color: $font-gray-color;
  font-weight: 500;
}

.not-decorate {
  text-decoration: none;
}

</style>