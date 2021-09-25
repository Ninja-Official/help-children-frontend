<template>
  <div class="nav-btn-link">
    <NuxtLink class="nav-btn" v-bind:to="route"> {{ buttonText }} </NuxtLink>
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
  text-decoration: none;
  color: rgb(107, 107, 107);
}

.nav-btn:hover {
  color: black;
}

.nav-btn-link {
  display: flex;
  justify-content: center; /* align horizontal */
  align-items: center;
}

</style>