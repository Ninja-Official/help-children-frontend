<template>
  <div class="date-container">
    <img src="../static/icon-calendar.svg">
    <p class="date"> {{ date }} </p>
  </div>
</template>

<script>
  export default {
    props: {
      date: {
        type: String,
        default: "12 ноября 2021"
      }
    }
  }
</script>

<style lang="scss" scoped>

@import "../assets/constants.scss";

.date-container {
  display: flex; 
  align-items: center;

  .date {
    font-size: $font-size-1;
    display: flex;
    justify-content: center;
    margin: 0;
  }
}

</style>