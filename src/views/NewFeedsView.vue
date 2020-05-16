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
      usernameIcon: 'https://instagram.fnbo1-1.fna.fbcdn.net/v/t51.2885-19/s150x150/80799187_439021066984282_4863388548130144256_n.jpg?_nc_ht=instagram.fnbo1-1.fna.fbcdn.net&_nc_ohc=S-6RqHcp9MEAX9tDG2I&oh=6246a0f7f0e1ba12a18cabcdb91f2e88&oe=5EE6CFBC',
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
