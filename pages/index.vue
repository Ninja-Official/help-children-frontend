<template>
  <PageBase>
    <h1 class="page-text page-title">
      Добро пожаловать на <br /><span class="page-title-bottom"
        >платформу <span class="highlighted-word">добрых</span> дел</span
      >
    </h1>
    <div class="map-block">
      <img
        :src="mapImage"
        alt=""
        srcset=""
        style="
          z-index: 99;
          filter: drop-shadow(0px 0px 15px rgba(0, 0, 0, 0.2));
        "
      />
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
      <div class="column">
        <h2 class="page-text info-title" style="text-align: left">
          Стань
          <span class="highlighted-word">одним</span> из нас
        </h2>
        <p
          class="page-text info-text"
          style="text-align: left; margin-bottom: 20px; padding-right: 10px"
        >
          Сейчас в реализации находятся еще<br />
          <span class="highlighted-word">{{ eventsTodoCount }}</span>
          мероприяий, и это только начало!
        </p>
        <img
          src="https://media.istockphoto.com/photos/happy-kid-in-glasses-holding-hands-up-picture-id1149081585?k=20&m=1149081585&s=612x612&w=0&h=CL6rSThOYQppuo1zMAv7T2Ps_ZBX_SzgNWmiVhLB-Ps="
          img-width="150"
          img-height="200"
          style="
          text-shadow: 1px 1px 2px #333; 
          border-radius: 20px 
          width: 150px; 
          height: 200px; 
          bject-fit: cover;"
        />
      </div>
      <div class="column">
        <img
          src="https://images.unsplash.com/photo-1489710437720-ebb67ec84dd2?ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8aGFwcHklMjBjaGlsZHxlbnwwfHwwfHw%3D&ixlib=rb-1.2.1&w=1000&q=80"
          img-width="150"
          img-height="330"
          style="
          text-shadow: 1px 1px 2px #333; 
          border-radius: 20px 
          width: 150px; 
          height: 330px; 
          bject-fit: cover;"
        />
      </div>
    </div>
    <div>
      <p
        class="page-text info-text"
        style="text-align: center; margin-bottom: 50px; margin-top: 50px"
      >
        <button class="start-help-button">
          <b>Хочу помочь</b>
        </button>
      </p>
    </div>
  </PageBase>
</template>

<style lang="scss">
@import "../assets/constants.scss";

.start-help-block {
  padding-top: 71px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.center {
  display: flex;
  justify-content: center;
  align-items: center;
}

.start-help-button {
  font-size: 18px;
  line-height: 32px;
  /* identical to box height, or 178% */

  align-items: center;

  color: $font-bright-color;

  width: 228.94px;
  height: 50px;

  padding: 0;
  border: none;

  background: $accent-color-red;
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
  color: $font-bold-color;
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
  text-shadow: 0px 4px 0 $font-bright-color;
  color: $accent-color-red;

  // display: inline;

  // background-color: #55efc4;

  // border-radius: 999px;
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
import mapImage from "~/assets/map.png";
export default {
  data() {
    return { mapImage };
  },
  computed: {
    usersCount() {
      return 1234567;
    },
    eventsCount() {
      return 957;
    },
    eventsTodoCount() {
      return 957;
    },
  },
};
</script>
