<template>
  <div class="container">
     <p>{{ text }}</p>
     <textarea v-bind:id="name" v-bind:name="name"></textarea>
  </div>
</template>

<script>

  export default {
    props: {
      text: {
        type: String,
        default: ""
      },
      name: {
        type: String,
        defautl: ""
      }
    }
  }
</script>

<style lang="scss" scoped>

.container {
  display: flex;
  gap: 15px;
}

p {
  margin: 0;
}

</style>