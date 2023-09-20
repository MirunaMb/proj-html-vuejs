<script>
import Button from "./components/Button.vue";

export default {
  data() {
  return {
    dropDowns: [
      {
        items: [
          { text: 'Home', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Games', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Shop', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Pages', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Blog', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Contact', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      
    ],
    components: { Button }
  };
},

};
</script>


<template>
  <div class="wrapper mt-5">
    <!-- Header Top -->
    <div class="header-top">
      <div class="logo"><img class="logo" src="/img/logo.png" alt="Logo">
      </div>
      <div class="button-container">
    <div v-for="(dropdown, index) in dropDowns" :key="index" class="dropdown">
      <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
        {{ dropdown.items[0].text }}
      </button>
      <ul class="dropdown-menu dropdown-menu-dark">
        <li v-for="(item, itemIndex) in dropdown.items" :key="itemIndex" :class="{ 'active': item.active }">
          <a class="dropdown-item" href="#" v-if="!item.divider">{{ item.text }}</a>
          <hr class="dropdown-divider" v-else-if="item.divider" />
        </li>
      </ul>
    </div>
      </div>
      <div class="live-streaming">
    <span>icon</span>
    <div>
    <Button >Il mio testo personalizzato</Button >
    </div>
      </div>
    </div>
    <!-- Header Top -->

    <!-- Header Left -->
    <div class="header-left">
      <img src="" alt="">joystick</img>
      <p></p>
      <h1></h1>
      <p></p>
      <button></button>
      <p>icon</p>
    </div>
    <!-- Header Left -->

    <!-- Header Right -->
    <div class="header-right">
    </div>
     <!-- Header Right -->
  </div>
</template>

<style lang="scss" scoped>
.wrapper{
  background-image: url('./img/game-details-banner-bg.png');
  background-size: cover;
  height: 100vh;
}
.button-container{
  display: flex;
  justify-content: flex-end; 
  margin: 10px;
}
.btn{
  margin-right: 10px;
  background-color: #94CB53;
}
</style>