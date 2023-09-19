<script>
import GameInfo from './GameInfo.vue'; 


export default {
  data() {
    return {
      title: "Game Info"
    }
  },

  components: {GameInfo },
};
</script>

<template>
  <h1>{{ title }}</h1>
  <GameInfo />
</template>

<style lang="scss" scoped></style>