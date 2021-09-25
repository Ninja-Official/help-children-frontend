<template>
  <nav>
    <TheAppLogo class="nav-el"/>
    <TheNavButtonsRoutesSection class="nav-el" />
    <TheAuthorizationSection class="nav-el" />
  </nav>
</template>

<script>

export default {

}

</script>

<style scoped>

nav {
  position: sticky;
  z-index: 100;
  top: 0px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: white;
  margin: 0;
  box-shadow: 0 4px 4px 0 rgba(0,0,0,.2);
}

.nav-el {
  margin: 5px;
  flex: 1;
}

</style>