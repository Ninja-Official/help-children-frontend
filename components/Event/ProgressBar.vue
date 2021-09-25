<template>
  <div class="container">
    <EventProgressPoint id="point-1" text="Что за мероприятие" ></EventProgressPoint> 
    <EventProgressPoint id="point-2" text="Подробное описание" ></EventProgressPoint> 
    <EventProgressPoint id="point-3" text="Место и дата" ></EventProgressPoint> 
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>

.container {
  display: flex;
  justify-content: space-around;
}

</style>