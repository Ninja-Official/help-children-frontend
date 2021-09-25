<template>
  <PageBase
    :style="{ backgroundImage: `url(${backgroundRectangleImage})` }"
    class="background-rectangle"
  >
    <h1 class="page-text page-title">
      Добро пожаловать на <br /><span class="page-title-bottom"
        >платформу <span class="highlighted-word">добрых</span> дел</span
      >
    </h1>
    <div class="map-block">
      <img :src="mapImage" alt="" srcset="" />
      <div class="map-text">
        <h2 class="page-text info-title" style="text-align: right">
          Нас уже <span class="highlighted-word">{{ usersCount }}</span>
        </h2>
        <p class="page-text info-text">
          Мы объединяем тех, кто нуждается <br />в помощи, с тем, кто может
          помочь!
        </p>
      </div>
    </div>
    <div class="image-slider-block">
      <h2 class="page-text info-title" style="text-align: center">
        Проведено
        <span class="highlighted-word">{{ eventsCount }}</span> мероприятий
      </h2>
      <p
        class="page-text info-text"
        style="text-align: center; margin-bottom: 20px"
      >
        Общими усилиями мы проводим<br />
        мероприятия по всей стране!
      </p>
      <b-carousel
        id="carousel-1"
        :interval="3000"
        controls
        background="#ababab"
        img-width="640"
        img-height="419"
        style="text-shadow: 1px 1px 2px #333; border-radius: 20px"
      >
        <!-- Text slides with image -->
        <b-carousel-slide
          img-src="https://picsum.photos/1024/480/?image=52"
        ></b-carousel-slide>

        <!-- Slides with custom text -->
        <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=54">
        </b-carousel-slide>

        <!-- Slides with image only -->
        <b-carousel-slide
          img-src="https://picsum.photos/1024/480/?image=58"
        ></b-carousel-slide>
      </b-carousel>
    </div>

    <div class="start-help-block">
      <button class="start-help-button">Я могу помочь</button>
    </div>
  </PageBase>
</template>

<style>
.start-help-block {
  padding-top: 71px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.start-help-button {
  font-size: 18px;
  line-height: 32px;
  /* identical to box height, or 178% */

  align-items: center;

  color: #ffffff;

  width: 228.94px;
  height: 50px;

  padding: 0;
  border: none;

  background: #ff4459;
  border-radius: 10px;
}

.image-slider-block {
  padding-top: 95px;
  padding-left: 88px;
  padding-right: 88px;
}

.carousel-inner {
  border-radius: 20px !important;
}

.page-text {
  /* font-family: Inter; */
  color: #2d3436;
}

.map-text {
  top: 42px;
  right: 88px;
  position: absolute;
}

.info-title {
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 32px;
  /* or 133% */
}

.info-text {
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 32px;
}

.page-title {
  padding-top: 57px;

  font-style: normal;
  font-weight: 800;
  font-size: 72px;
  line-height: 65px;

  text-align: center;
  letter-spacing: -3px;
}

.page-title-bottom {
  font-size: 48px;
}

.highlighted-word {
  text-shadow: 0px 4px 0 #fff;
  color: #ff4459;
}

.background-rectangle {
  background-position: right top;
  background-repeat: no-repeat;
  background-attachment: inherit;
  background-size: 50%;
}

.map-block {
  position: relative;

  padding-top: 54px;
  padding-left: 88px;
  padding-right: 88px;

  display: flex;
  align-items: center;
  justify-content: center;
}
</style>

<script>
import backgroundRectangleImage from "~/assets/rectangle.png";
import mapImage from "~/assets/map.png";
export default {
  data() {
    return { backgroundRectangleImage, mapImage };
  },
  computed: {
    usersCount() {
      return 1234567;
    },
    eventsCount() {
      return 957;
    },
  },
};
</script>
