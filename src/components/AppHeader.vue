<script>

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
    };
  },

};
</script>


<template>
  <div class="wrapper ">
    <!-- Header Top -->
    <div class="header-top">
      <div class="logo"><img class="logo" src="/img/logo.png" alt="Logo">
      </div>
      <div class="live-streaming d-flex">
        <div class="button-container">
          <div v-for="(dropdown, index) in dropDowns" :key="index" class="dropdown">
            <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown"
              aria-expanded="false">
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
        <img class="cart-icon" src="/img/icon/cart-icon.png" alt="cart">
        <button class="green-button">LIVE STREAMING</button>
      </div>
    </div>
    <!-- Header Top -->

    <!-- CONTAINER HEADER COLS -->
    <div class="header-cols">
      <!-- Header Left -->
      <div class="header-left ">
        <div>
          <img src="/img/game-controler-2.png" class="w-50" alt="">
        </div>
        <div class="game-text">
          <p class="title ">Game With Live Streaming</p>
          <h1 class="description ">Future Of Esports</h1>
          <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi sapiente itaque dicta. Inventore
            explicabo nihil alias ipsum consequuntur facilis cumque.</p>
          <div class="button-icon d-flex">
            <button class="green-button">EXPLORE GAMES</button>
            <div class="play-button">
              <img src="/img/icon/play-icon.png" alt="Play">
            </div>
          </div>
        </div>

      </div>
      <!-- Header Left -->

      <!-- Header Right -->
      <div class="header-right">
        <div>
          <img src="/img/index-banner-illus.png" alt="">
        </div>
      </div>
      <!-- Header Right -->
    </div>
  </div>
</template>

<style lang="scss" scoped>
.wrapper {
  background-image: url('./img/game-details-banner-bg.png');
  background-size: cover;
  height: 100vh;
  min-height: 100vh;
}

// HEADER TOP
.header-top {
  display: flex;
  justify-content: space-between;
}

.button-container {
  display: flex;
  justify-content: flex-end;
  margin: 10px;
}

.btn {
  margin-right: 10px;
  background-color: #94CB53;
}

.green-button {
  width: 10rem;
  height: 3rem;
  background: #06ca7c;
  border-color: #06ca7c;
  display: flex;
  align-items: center;
  color: #f0ede6;
  font-size: large;
  line-height: 4rem;
  border-radius: 70px;
}

.cart-icon {
  width: 40px;
  height: 40px;
  margin: 10px;
}

// HEADER COLS 
.header-cols {
  min-width: 500px;
  min-height: 500vh;
  display: flex;
  margin-top: 150px;
}

// HEADER LEFT
.header-left {
  width: 50%;
  height: 100vh;
  position: relative;
  margin-top: 200px;
}

.game-text {
  position: absolute;
  left: 20%;
  bottom: 65%;
}


.title {
  color: #93c067;

}

.description,
.text {
  color: white;

}

.button-icon {
  width: 300px;
  justify-content: space-evenly;

}

.play-button {
  display: inline-block;
  width: 64px;
  height: 60px;
  border: 4px solid #ccc;
  border-radius: 50%;
  background-color: white;
  text-align: center;
  line-height: 64px;
}

.play-button img {
  width: 30%;
  height: auto;
  margin-bottom: 15px;
}

// HEADER RIGHT
</style>