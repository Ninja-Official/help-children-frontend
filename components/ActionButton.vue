<template>
  <div class="accent-button">
    Хочу участвовать!
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>

@import "../assets/constants.scss";

.accent-button {
  margin: 15px 20px;
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