<template>
  <NuxtLink v-bind:to="'/events/'+ id">
    <div class="card">
      <h2 class="text"> {{ name }} </h2>
      <p class="text"> {{ date }} </p>
    </div>
  </NuxtLink>
</template>

<script>
  export default {
    props: {
      id: {
        type: Number,
        default: 0
      },
      name: {
        type: String,
        default: "Название события"
      },
      date: {
        type: String,
        default: "01-01-2022"
      }
    }
  }
</script>

<style scoped>

.card {
  width: 300px;
  height: 150px;
  border-radius: 15px;
  background-color: teal;
  margin: 30px;
}

.card:hover {
  background-color: rgb(0, 66, 66);
}

.text {
  margin-left: 10px;
  color: white;
}

</style>