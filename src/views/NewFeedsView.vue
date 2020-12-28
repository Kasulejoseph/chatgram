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
      usernameIcon: 'https://instagram.fnbo1-1.fna.fbcdn.net/v/t51.2885-19/s150x150/113725555_668836093702661_6353173893857121562_n.jpg?_nc_ht=instagram.fnbo1-1.fna.fbcdn.net&_nc_ohc=d40obwK0oZMAX_zmcCx&tp=1&oh=76d15b8b08a62f424c0b3d7f7b99b711&oe=60140714',
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
