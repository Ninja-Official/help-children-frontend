<template>
  <nav>
    <NuxtLink class="nav-el" to="/home">Home</NuxtLink>
    <NuxtLink class="nav-el" to="/main">Main</NuxtLink>
  </nav>
</template>

<script>

export default {

}

</script>

<style scoped>

nav {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: darkslategrey;
  margin: 0;
}

.nav-el {
  margin: 5px;
  flex: 1;
}

</style>