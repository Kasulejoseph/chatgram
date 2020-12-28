<template>
  <div id="app">
    <nav class="border-bottom">
      <NavBar />
    </nav>
    <main class="row main">
      <section class="col-8 p-0">
        <trendfeeds></trendfeeds>
        <div class="mt-5">
          <newfeeds></newfeeds>
        </div>
      </section>
      <section class="col ml-4 p-0 mt-5">
        <Suggestions/>
      </section>
    </main>
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import TrendFeeds from "./components/TrendFeeds";
import NewFeedsView from "./views/NewFeedsView"
import Suggestions from './components/Suggestions'

export default {
  name: "App",
  components: {
    NavBar,
    Suggestions,
    trendfeeds: TrendFeeds,
    newfeeds: NewFeedsView
  }
};
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
}
.main {
  width: 100%;
  max-width: 72%;
  margin: 0 auto;
  position: relative;
}
</style>
