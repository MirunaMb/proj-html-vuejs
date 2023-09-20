<script>
import AppHeader from './components/AppHeader.vue';
import Battle from './components/Battle.vue';
import TrendingBattle from './components/TrendingBattle.vue';
import FutioFacts from './components/FutioFacts.vue';
import LiveStreaming from './components/LiveStreaming.vue';
import FutioFeedback from './components/FutioFeedback.vue';
import LatestNews from './components/LatestNews.vue';
// import Footer from './components/Footer.vue';




export default {
  data() {
    return {
    }
  },
  components: { AppHeader, Battle, TrendingBattle, FutioFacts, LiveStreaming, FutioFeedback, LatestNews, },
};
</script>

<template>
  <AppHeader />
  <Battle />
  <TrendingBattle />
  <FutioFacts />
  <LiveStreaming />
  <FutioFeedback />
  <LatestNews />
</template>

<style lang="scss" >
@use './styles/general.scss' as *;
</style>