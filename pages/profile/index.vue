<template>
  <div>
    <PageBase>
      <b-container class="bv-example-row">
        <b-row>
          <b-col> <ProfileInfoCard /></b-col>
          <b-col cols="8">
            <div class="profile-block" style="padding: 10px; display: grid">
              <div class="title-with-link">
                <span class="block-title">Мои достижения</span>
                <span class="block-title-link">Посмотерть все (23)</span>
              </div>
              <div id="achievements">
                <div class="achievement">
                  <img
                    class="achievement-img"
                    src="https://via.placeholder.com/100x100"
                  />
                </div>
                <div class="achievement">
                  <img
                    class="achievement-img"
                    src="https://via.placeholder.com/100x100"
                  />
                </div>
                <div class="achievement">
                  <img
                    class="achievement-img"
                    src="https://via.placeholder.com/100x100"
                  />
                </div>
                <div class="achievement">
                  <img
                    class="achievement-img"
                    src="https://via.placeholder.com/100x100"
                  />
                </div>
              </div>
            </div>
            <div class="profile-block">
              <div style="padding-bottom: 50px">
                <span class="block-title" style="padding: 10px">Мои цели</span>
              </div>
              <div class="goal-card">
                <div id="goal-progress">
                  <progress
                    value="10"
                    max="100"
                    id="goal-progressbar"
                  ></progress>
                  <span id="progress-text">10% пройдено</span>
                </div>
                <h2 id="goal-name">Путь web-дизайнера</h2>
                <div id="goal-stats">
                  <span class="goal-stats-text"
                    ><svg
                      class="goal-stats-icon"
                      width="15"
                      height="10"
                      viewBox="0 0 15 10"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M13.5125 1.0625L4.8844 9.3125L0.962524 5.5625"
                        stroke="white"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      />
                    </svg>
                    3 задания выполнено
                  </span>

                  <span class="goal-stats-text"
                    ><svg
                      class="goal-stats-icon"
                      width="18"
                      height="16"
                      viewBox="0 0 18 16"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M9.17505 1.0625L11.5988 5.7575L17.0188 6.515L13.0969 10.1675L14.0225 15.3275L9.17505 12.89L4.32761 15.3275L5.25317 10.1675L1.3313 6.515L6.75133 5.7575L9.17505 1.0625Z"
                        stroke="white"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      />
                    </svg>

                    2 награды
                  </span>
                </div>
                <button id="goal-continue-button">Продолжить</button>
              </div>
            </div>
            <div class="profile-block">
              <div style="padding-bottom: 20px; display: grid">
                <h2 class="block-title" style="padding: 10px">
                  Персональные рекомендации
                </h2>
                <div
                  class="title-with-link"
                  style="padding-left: 10px; padding-right: 10px"
                >
                  <span class="block-subtitle">Обучение</span>
                  <span class="block-title-link">Посмотерть все (23)</span>
                </div>
              </div>
              <img
                class="image-block"
                src="https://via.placeholder.com/502x290"
              />
              <div class="event-info">
                <svg
                  width="30"
                  height="30"
                  viewBox="0 0 30 30"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M15 22.5C19.1421 22.5 22.5 19.1421 22.5 15C22.5 10.8579 19.1421 7.5 15 7.5C10.8579 7.5 7.5 10.8579 7.5 15C7.5 19.1421 10.8579 22.5 15 22.5Z"
                    stroke="#575D5E"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M15 10.5V15L18 16.5"
                    stroke="#575D5E"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  /></svg
                ><span class="event-time-text">23 марта 2021</span>
                <p class="event-title">
                  Курсы по Figma от Александра Наташкина
                </p>
                <button class="event-button">Хочу участвовать</button>
              </div>
            </div>

            <div class="profile-block">
              <div style="padding-bottom: 20px; display: grid">
                <div
                  class="title-with-link"
                  style="padding-left: 10px; padding-right: 10px"
                >
                  <span class="block-subtitle">Мероприятия</span>
                  <span class="block-title-link">Посмотерть все (23)</span>
                </div>
              </div>
              <img
                class="image-block"
                src="https://via.placeholder.com/502x290"
              />
              <div class="event-info">
                <svg
                  width="30"
                  height="30"
                  viewBox="0 0 30 30"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M15 22.5C19.1421 22.5 22.5 19.1421 22.5 15C22.5 10.8579 19.1421 7.5 15 7.5C10.8579 7.5 7.5 10.8579 7.5 15C7.5 19.1421 10.8579 22.5 15 22.5Z"
                    stroke="#575D5E"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M15 10.5V15L18 16.5"
                    stroke="#575D5E"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  /></svg
                ><span class="event-time-text">23 марта 2021</span>
                <p class="event-title">Выставка «Body Worlds. Мир тела»</p>
                <svg
                  width="30"
                  height="30"
                  viewBox="0 0 30 30"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M21.75 13.5C21.75 18.75 15 23.25 15 23.25C15 23.25 8.25 18.75 8.25 13.5C8.25 11.7098 8.96116 9.9929 10.227 8.72703C11.4929 7.46116 13.2098 6.75 15 6.75C16.7902 6.75 18.5071 7.46116 19.773 8.72703C21.0388 9.9929 21.75 11.7098 21.75 13.5Z"
                    stroke="#575D5E"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M15 15.75C16.2426 15.75 17.25 14.7426 17.25 13.5C17.25 12.2574 16.2426 11.25 15 11.25C13.7574 11.25 12.75 12.2574 12.75 13.5C12.75 14.7426 13.7574 15.75 15 15.75Z"
                    stroke="#575D5E"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  /></svg
                ><span class="event-time-text"
                  >г. Москва, ВДНХ, павильон 21</span
                >

                <button class="event-button">Хочу участвовать</button>
              </div>
            </div>
          </b-col>
        </b-row>
      </b-container>
    </PageBase>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../../assets/constants.scss";

.event-button {
  font-size: 18px;
  width: 100%;
  margin-top: 20px;
  align-items: center;

  color: $font-bright-color;

  height: 50px;

  padding: 0;
  border: none;

  background: $accent-color-red;
  border-radius: 10px;
}

.event-title {
  margin: 0;
  padding-left: 5px;
  padding-top: 3px;
  font-family: Inter;
  font-weight: bold;
  font-size: 18px;

  color: #2d3436;
}

.event-time-text {
  position: relative;
  top: 1px;
  font-family: Inter;

  font-weight: 500;
  font-size: 14px;
  line-height: 32px;

  color: rgba(45, 52, 54, 0.8);
}

.event-info {
  padding: 14px 26px 14px 26px;
}

.image-block {
  width: 100%;
  height: 290px;
  border-radius: 20px 20px 0px 0px;
}

.title-with-link {
  padding-top: 10px;
  width: 100%;
  text-align: right;
}

#goal-progressbar {
  margin-right: 10px;
  width: 75%;
}

#goal-continue-button {
  font-size: 18px;
  width: 203px;
  margin-top: 23px;
  align-items: center;

  color: $accent-color-red;

  height: 50px;

  padding: 0;
  border: none;

  background: $font-bright-color;
  border-radius: 10px;
}

.goal-stats-icon {
  margin: 5px;
}

.goal-stats-text {
  padding-right: 38.7px;
  font-family: Inter;
  font-weight: normal;
  font-size: 12px;

  color: #ffffff;
}

#goal-name {
  font-family: Inter;
  font-weight: bold;
  font-size: 36px;

  padding-top: 25.5px;

  color: #ffffff;
}

#progress-text {
  font-family: Inter;
  font-weight: bold;
  font-size: 14px;

  color: #ffffff;
}

#goal-progress {
  padding-top: 30px;
}

progress {
  border: none;
  height: 15px;
  width: 100%;
  background: #55efc4;
}

progress {
  color: lightblue;
}

progress::-webkit-progress-value {
  background: lightblue;
}

progress::-moz-progress-bar {
  background: #fff;
}

progress::-webkit-progress-value {
  background: #55efc4;
}

progress::-webkit-progress-bar {
  background: #fff;
}
.goal-card {
  padding: 10px;
  height: 255px;
  background-color: #ff4459;

  background: #ff4459;
  border-radius: 10px;
}

.block-title-link {
  font-family: Inter;
  font-weight: normal;
  font-size: 18px;

  color: #ff4459;
}

.block-subtitle {
  float: left;
  font-family: Inter;
  font-weight: bold;
  font-size: 18px;

  color: #2d3436;
}

.block-title {
  float: left;
  font-family: Inter;
  font-weight: bold;
  font-size: 24px;

  color: #2d3436;
}

#achievements {
  display: inline-flex;
}
.achievement {
  padding-right: 19px;
  margin-top: 5px;
}

.achievement-img {
  width: 100px;
  height: 100px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.1);
  border-radius: 9999px;
}

.profile-block {
  background: #ffffff;
  box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.25);
  border-radius: 10px;
  margin-bottom: 23px;
}
</style>
