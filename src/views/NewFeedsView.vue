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
      usernameIcon: 'https://instagram.fnbo1-1.fna.fbcdn.net/v/t51.2885-19/s150x150/66507740_2389120978080254_9153918996884488192_n.jpg?_nc_ht=instagram.fnbo1-1.fna.fbcdn.net&_nc_ohc=rDc5swnFrBMAX8ydNp_&oh=83a277523fd96dd479232a3bf8808079&oe=5EE64FE4',
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
