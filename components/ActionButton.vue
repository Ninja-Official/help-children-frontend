<template>
  <div class="accent-button">
    {{ buttonText }}
    <img v-if="buttonImage !== ''" v-bind:src="buttonImage">
  </div>
</template>

<script>
  export default {
    props: {
      buttonText: {
        type: String,
        default: ""
      },
      buttonImage: {
        type: String,
        default: ""
      }
    }
  }
</script>

<style lang="scss" scoped>

@import "../assets/constants.scss";

.accent-button {
  display: flex;
  justify-content: center; 
  align-items: center;
  color: $font-bright-color;
  background-color: $accent-color-red;
  border-radius: $main-border-radius;
  height: 50px;
  font-weight: bold;
}

</style>