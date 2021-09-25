<template>
  <div
    id="profile-card"
    :style="{
      'background-image': 'url(' + require('~/assets/wave.png') + ')',
    }"
  >
    <div id="user-info">
      <div class="avatar">
        <img class="avatar-image" src="https://via.placeholder.com/64x64" />
      </div>
      <div>
        <p class="name">Иван Иванов</p>
        <p class="user-type">Воспитанник</p>
      </div>
    </div>
    <div class="user-stats">
      <div class="stats-line">
        <div class="stats-line-text">
          <span class="stats-text">Мероприятия</span>
          <span class="stats-number">3</span>
        </div>
      </div>
      <hr />
      <div class="stats-line">
        <div class="stats-line-text">
          <span class="stats-text">Часов обучения</span>
          <span class="stats-number">25</span>
        </div>
      </div>

      <div id="profile-fullness">
        <span class="stats-text" style="margin-right: 4px"
          >Заполнение профиля:</span
        >
        <span class="stats-number">56%</span>
      </div>
      <meter value="56" max="100" low="10" high="60">Нормальная</meter>
    </div>
    <button class="card-button" style="margin-bottom: 10px; margin-top: 15px">
      Я хочу
    </button>
    <button class="card-button">Пройти профориентацию</button>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../assets/constants.scss";
.card-button {
  font-size: 18px;

  align-items: center;

  color: $font-bright-color;

  width: 100%;
  height: 50px;

  padding: 0;
  border: none;

  background: $accent-color-red;
  border-radius: 10px;
}
meter {
  width: 100%;
}
meter::-webkit-meter-optimum-value {
  background: #55efc4;
}
#profile-fullness {
  padding-top: 40px;
  display: flex;
}
hr {
  margin-top: 10px;
  margin-bottom: 10px;
  border: 0;
  border-top: 1px solid rgba(45, 52, 54, 0.8);
}
.stats-number {
  font-weight: 600;
  font-size: 12px;

  color: rgba(45, 52, 54, 0.8);
}
.stats-text {
  font-family: Inter;
  float: left;
  font-weight: 300;
  font-size: 12px;

  color: rgba(45, 52, 54, 0.8);
}
.stats-line {
  width: 100%;
  height: 30px;
  line-height: 30px;
  overflow: hidden;
  text-align: justify;
}
.stats-line-text {
  width: 100%;
  height: 30px;
  text-align: right;
}
.name {
  padding-top: 10px;
  margin: 0;
  font-family: Inter;
  font-size: 18px;

  color: $font-bold-color;
}
.user-type {
  margin: 0;
  font-family: Inter;
  font-size: 12px;

  color: #3c4547c2;
}
#user-info {
  display: inline-flex;
  margin-bottom: 23px;
}
.avatar {
  width: 64px;
  height: 64px;
  margin-right: 21px;
}
.avatar-image {
  width: 64px;
  height: 64px;
  border-radius: 999px;
}
#profile-card {
  width: 297px;
  height: 465px;
  background-position: top;
  background-repeat: no-repeat;
  background-size: auto;
  background-color: #fff;
  box-shadow: 0px 0px 15px rgb(0 0 0 / 25%);
  border-radius: 10px;

  padding-top: 70px;
  padding-left: 21px;
  padding-right: 21px;
}
</style>