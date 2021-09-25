<template>
  <div class="buttons-section">
    <NavButton button-text="Главная" route="/" />
    <NavCircleSeparator />
    <NavButton button-text="Мероприятия" route="/events" />
    <NavCircleSeparator />
    <NavButton button-text="Сообщения" route="/messenger" />
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

.buttons-section {
  display: flex;
  justify-content: center;
  align-content: center;
  gap: 15px;
}

</style>