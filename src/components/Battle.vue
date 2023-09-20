<script>
// import MyComponent from "./components/MyComponent.vue";

export default {
};
</script>

<template>
    <div class="wrapper mt-5">
        <div class="header-cols">
            <div class="header-left ">
                <img src="/img/features-illus.png" alt="">
            </div>
            <div class="header-right">
                <div class="game-text">
                    <h2 class="title ">The Ultimate Competitive Gaming Platform</h2>
                    <h1 class="text ">Make Your Mark On The Battle Field</h1>
                    <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi sapiente itaque dicta.
                        Inventore
                        explicabo nihil alias ipsum consequuntur facilis cumque.</p>
                    <div class="game-plan d-flex">
                        <div>
                            <img src="/img/icon/features-icon-1.png" alt="">
                        </div>
                        <div>
                            <h1 class="text ">Live Streaming</h1>
                            <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi sapiente itaque
                                dicta.
                                Inventore
                                explicabo nihil alias ipsum consequuntur facilis cumque.</p>
                        </div>
                    </div>
                    <div class="game-plan d-flex">
                        <div>
                            <img src="/img/icon/features-icon-2.png" alt="">
                        </div>
                        <div>
                            <h1 class="text ">Great Tournament</h1>
                            <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi sapiente itaque
                                dicta.
                                Inventore
                                explicabo nihil alias ipsum consequuntur facilis cumque.</p>
                        </div>
                    </div>
                    <div class="game-plan d-flex">
                        <div>
                            <img src="/img/icon/features-icon-3.png" alt="">
                        </div>
                        <div>
                            <h1 class="text ">Gaming News</h1>
                            <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi sapiente itaque
                                dicta.
                                Inventore
                                explicabo nihil alias ipsum consequuntur facilis cumque.</p>
                        </div>
                    </div>


                    <div class="button-icon d-flex">
                        <button class="green-button">EXPLORE GAMES</button>
                    </div>
                </div>
            </div>

        </div>
    </div>
</template>
  

<style lang="scss" scoped>
.wrapper {
    background-color: black;
    height: 100vh;
    min-height: 100vh;
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
    height: 100%;
    margin-top: 200px;
}

.title {
    color: #93c067;
    width: 300px;
}

.description,
.text {
    color: white;
    padding: 10px;

}

.game-text {
    margin-top: 200px;
}

.button-icon {
    width: 300px;
    justify-content: space-evenly;

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
</style>