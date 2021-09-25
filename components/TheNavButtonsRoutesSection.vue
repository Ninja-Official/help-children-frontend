<template>
  <div class="buttons-section">
    <NavButton button-text="Главная" route="/home" />
    <NavCircleSeparator />
    <NavButton button-text="Мероприятия" route="/events" />
    <NavCircleSeparator />
    <NavButton button-text="Галерея" route="/chat" />
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
}

</style>