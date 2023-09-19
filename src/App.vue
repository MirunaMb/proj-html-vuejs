<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  data() {
    return {
      title: "Hello world"
    }
  },
  components: {AppHeader, AppMain,AppFooter },
};
</script>

<template>
  <h1>{{ title }}</h1>
  <AppHeader  />
  <AppMain />
  <AppFooter />

</template>

<style lang="scss" >
@use './styles/general.scss' as *;
</style>