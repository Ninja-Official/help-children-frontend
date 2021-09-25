<template>
  <div class="content-page">
    <div class="page-back">

    </div>
    <div class="content-container">
      <slot>

      </slot>
    </div>
    <div class="page-back">
      
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

html,
body {
  height: 100%;
  margin: 0;
}

.content-page {
  display: flex;
  height: 100vh;
  justify-content: center;
}

.page-back {
  background-color: #ececec;
  flex: 2;
  flex-shrink: 3;
}

.content-container {
  flex: 8;
  flex-shrink: 0;
}

</style>