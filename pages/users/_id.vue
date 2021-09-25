<template>
  <PageBase>
    <div>
      There is gonna be LK of user#{{ id }}
    </div>
  </PageBase>
</template>

<script>
  export default {
    validate ({ params }) {
      return /^\d+$/.test(params.id) // + get запрос на наличие в базе
    },
    computed: {
      id () {
        return this.$route.params.id
      }
    }
  }
</script>

<style scoped>

</style>