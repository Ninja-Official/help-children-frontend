<template>
  <div
    class="content-page"
    :style="{
      background:
        'url(' +
        require('~/assets/rectangle_right.png') +
        ') no-repeat 80% -70% scroll, url(' +
        require('~/assets/rectangle_left.png') +
        ') no-repeat 18% 50% scroll',
    }"
  >
    <div class="page-back"></div>
    <div class="content-container background-rectangle">
      <slot> </slot>
    </div>
    <div class="page-back"></div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
html,
body {
  height: 100%;
  margin: 0;
}

.content-page {
  display: flex;
  min-height: 100vh;
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

.background-rectangle {
  background-image: url("~/assets/wave_footer.png");
  background-repeat: no-repeat;
  background-attachment: scroll;
  background-size: contain;
  background-position: bottom center;
}
</style>

<script>
import backgroundRectangleRightImage from "~/assets/rectangle_right.png";
import backgroundRectangleLeftImage from "~/assets/rectangle_left.png";
import backgroundWaveFooterImage from "~/assets/wave_footer.png";
export default {
  data() {
    return {
      backgroundRectangleRightImage,
      backgroundRectangleLeftImage,
      backgroundWaveFooterImage,
    };
  },
};
</script>