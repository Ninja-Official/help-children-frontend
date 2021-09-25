<template>
  <ProfileCard>
    <div style="padding-bottom: 20px; display: grid">
      <div
        class="title-with-link"
        style="padding-left: 10px; padding-right: 10px"
      >
        <span class="block-subtitle">Мероприятия</span>
        <span class="block-title-link">Посмотерть все (23)</span>
      </div>
    </div>
    <img class="image-block" src="https://via.placeholder.com/502x290" />
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
      ><span class="event-time-text">г. Москва, ВДНХ, павильон 21</span>
      <ActionButton buttonText="Хочу участвовать" />
    </div>
  </ProfileCard>
</template>

<style lang="scss" scoped>
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
</style>