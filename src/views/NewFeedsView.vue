<template>
  <div>
    <NewFeeds
    :username="username"
    :usernameIcon="usernameIcon"
    :media="media"
    :statitics="statitics"
    :details="details"
    :duration="duration"
    />
    <NewFeeds
    class="mt-4"
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
import NewFeeds from '../components/NewFeeds'
import video from '../assets/video.png'

  export default {
    name: 'NewFeedsView',
    components: {
      NewFeeds
    },
    setup() {
      return {
        username: 'kawowosports',
        usernameIcon: '<i class="far fa-user-circle fa-2x"></i>',
        media: video,
        statitics: '5 views',
        details: 'This was the original FIFA/PES.',
        duration: '1 day'
      }
    }
    
  }
</script>

<style scoped>

</style>
