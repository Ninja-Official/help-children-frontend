<template>
  <div class="nav-btn">
    <NuxtLink v-bind:to="route"> {{ buttonText }} </NuxtLink>
  </div>
</template>

<script>
  export default {
    props: {
      buttonText: {
        type: String, 
        default: ""
      },
      route: {
        type: String,
        default: "/"
      }
    }
  }
</script>

<style scoped>

.nav-btn {

}

</style>