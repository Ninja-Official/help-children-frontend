<template>
  <div>
    <ProfileCard style="padding: 10px; display: grid">
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
    </ProfileCard>
  </div>
</template>


<style lang="scss" scoped>
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
</style>