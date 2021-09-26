<template>
  <div class="auth-block">
    <!-- <TheLoginButton />
    <TheRegistrationButton /> -->
    <NuxtLink to="/profile" style="display: flex">
      <img class="avatar" src="~/assets/avatar.png" />
      <p class="username">Иванов Иван</p>
    </NuxtLink>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.auth-block {
  margin-left: 50px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.username {
  padding-top: 15px;
  padding-left: 2px;
  width: 115px;
  font-size: 18px;
  line-height: 32px;
  text-align: center;
  color: rgba(45, 52, 54, 1);
}
.avatar {
  width: 64px;
  height: 64px;
  border-radius: 999px;
  border-style: solid;
  border-width: 2px;
  border-style: solid;
  border-color: rgba(61.92, 176.12, 200.81, 1);
}
</style>