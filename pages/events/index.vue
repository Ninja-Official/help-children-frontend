<template>
  <div>
    <PageBase>
      <div class="cards-holder">
        <EventCard name="Test"/>
        <EventCard name="Test2"/>
      </div>
    </PageBase>
    <TheCreateEventButton />
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

.cards-holder {
  display: flex;
  flex-wrap: wrap;
}

</style>