<template>
  <NuxtLink to="/events/create">
    <div class="crt-button">
      <div class="circle">
    
      </div>
    </div>
  </NuxtLink>
</template>

<script>
  export default {

  }
</script>

<style scoped>

.crt-button {
  position: absolute;
  right: 200px;
  bottom: 200px;
}

.circle:hover {
  background-color: rgb(29, 131, 83);
}

.circle {
  border-radius: 50%;
  width: 50px;
  height: 50px;
  background-color: rgb(42, 199, 126);
  position: relative;
}

.circle::after {
  content: " ";
  position: absolute;
  display: block;
  background-color: #fff;
  height: 5px;
  margin-top: -2.5px;
  top: 50%;
  left: 8px;
  right: 8px;
  z-index: 9;
}
.circle::before {
  content: " ";
  position: absolute;
  display: block;
  background-color: #fff;
  width: 5px;
  margin-left: -2.5px;
  left: 50%;
  top: 8px;
  bottom: 8px;
  z-index: 9;
}

</style>