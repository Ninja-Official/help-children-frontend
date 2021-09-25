<template>
  <div class="location-container">
    <img src="../static/icon-map-pin.svg">
    <p class="location"> {{ location }} </p>
  </div>
</template>

<script>
  export default {
    props: {
      location: {
        type: String,
        default: "12 ВДНХ д1"
      }
    }
  }
</script>

<style lang="scss" scoped>

@import "../assets/constants.scss";

.location-container {
  display: flex;

  .location {
    font-size: $font-size-1;
    display: flex;
    justify-content: center;
    margin: 0;
  }
}

</style>