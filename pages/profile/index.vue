<template>
  <div>
    <PageBase>
      <b-container class="bv-example-row">
        <b-row>
          <b-col> <ProfileInfoCard /></b-col>
          <b-col cols="8">
            <AchievementsCard />
            <GoalsCard />
            <EventCard />
          </b-col>
        </b-row>
      </b-container>
    </PageBase>
  </div>
</template>

<script>
export default {
  components: {
    AchievementsCard: () => {
      return import("~/components/profile/AchievementsCard.vue"); //указать нужный путь
    },
    GoalsCard: () => {
      return import("~/components/profile/GoalsCard.vue"); //указать нужный путь
    },
    EventCard: () => {
      return import("~/components/profile/EventCard.vue"); //указать нужный путь
    },
  },
};
</script>

<style lang="scss">
@import "../../assets/constants.scss";
</style>
