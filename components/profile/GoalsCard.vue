<template>
  <ProfileCard>
    <div style="padding-bottom: 50px">
      <span class="block-title" style="padding: 10px">Мои цели</span>
    </div>
    <div class="goal-card">
      <div id="goal-progress">
        <progress value="10" max="100" id="goal-progressbar"></progress>
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
  </ProfileCard>
</template>

<style lang="scss" scoped>
@import "../../assets/constants.scss";

.block-title {
  float: left;
  font-family: Inter;
  font-weight: bold;
  font-size: 24px;

  color: #2d3436;
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
</style>