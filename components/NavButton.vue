<template>
  <div class="nav-btn-link">
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

.nav-btn-link {
  display: flex;
  justify-content: center; /* align horizontal */
  align-items: center;
}

</style>