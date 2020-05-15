<template>
  <div>
    <NewFeeds
      class="mb-4"
      v-for="data in feeds"
      :key="data.id"
      :username="username"
      :usernameIcon="usernameIcon"
      :media="media"
      :statitics="statitics"
      :details="details"
      :duration="duration"
    />
  </div>
</template>

<script>
import NewFeeds from "../components/NewFeeds";
import video from "../assets/video.png";

export default {
  name: "NewFeedsView",
  components: {
    NewFeeds
  },
  setup() {
    const feeds = [{ id: 1 }, { id: 2 }, { id: 3 }];
    return {
      username: "kawowosports",
      usernameIcon: '<i class="far fa-user-circle fa-2x"></i>',
      media: video,
      statitics: "5 views",
      details: "This was the original FIFA/PES.",
      duration: "1 day",
      feeds
    };
  }
};
</script>

<style scoped></style>
