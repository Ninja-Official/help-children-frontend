<template>
  <nav>
    <NavButton class="nav-el" button-text="Главная" route="/home" />
    <NavButton class="nav-el" button-text="События" route="/events" />
    <NavButton class="nav-el" button-text="Общение" route="/chat" />
    <NavButton class="nav-el" button-text="Помощь" route="/help" />
    <TheRegistrationButton class="nav-el" />
    <TheLoginButton class="nav-el" />
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
  background-color: rgb(202, 222, 233);
  margin: 0;
}

.nav-el {
  margin: 5px;
  flex: 1;
}

</style>