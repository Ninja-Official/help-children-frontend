<template>
  <div class="container">
    <div v-bind:id="id" class="circle active" />
    <p> {{text}} </p>
  </div>
</template>

<script>
  export default {
    props: {
      text: {
        type: String,
        default: ""
      },
      state: {
        type: String,
        default: "inactive"
      },
      id: {
        type: String,
      }
    }
  }
</script>

<style lang="scss" scoped>

.container {
  display: flex;
  justify-content: start;
  align-items: center;
}

.circle {
  margin: 10px 5px 10px 5px;
  min-height: 10px;
  min-width: 10px;
  border-radius: 50%;
}

.active {
  background-color: #FF4459;
}

.inactive {
  background-color: #808080;
}

p {
  margin: 0;
}

</style>