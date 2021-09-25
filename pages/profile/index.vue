<template>
  <div>
    <PageBase>
      <div class="content">
        <b-container class="bv-example-row">
          <b-row>
            <b-col> <ProfileInfoCard /></b-col>
            <b-col cols="8">
              <AchievementsCard />
              <GoalsCard />
              <RecomendsCard />
              <EventCard />
            </b-col>
          </b-row>
        </b-container>
      </div>
    </PageBase>
  </div>
</template>

<script>
export default {
  components: {
    AchievementsCard: () => {
      return import("~/components/profile/AchievementsCard.vue");
    },
    GoalsCard: () => {
      return import("~/components/profile/GoalsCard.vue");
    },
    EventCard: () => {
      return import("~/components/profile/EventCard.vue");
    },
    RecomendsCard: () => {
      return import("~/components/profile/RecomendsCard.vue");
    },
  },
};
</script>

<style lang="scss">
@import "../../assets/constants.scss";

.content {
  padding-top: 40px;
}
</style>
