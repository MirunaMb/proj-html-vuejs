<script>


export default {
};
</script>

<template>
    <div class="wrapper">
        <div class="d-flex flex-column align-items-center py-5">
            <h1 class="title ">Trending Battle</h1>
            <h1 class="description ">Keep Eyes & Manage Upcoming</h1>
            <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi sapiente itaque dicta. Inventore
                explicabo nihil alias ipsum consequuntur facilis cumque.
            </p>
        </div>

        <div class="container-cards d-flex">
            <!-- CARD -->
            <div class="card">
                <div class="card-top d-flex justify-content-between py-4 px-4 ">
                    <div><img src="/img/game-img-1.png" alt="">

                    </div>
                    <div><img src="/img/verus-icon.png" alt="">
                    </div>
                    <div><img src="/img/game-img-2.png" alt="">
                    </div>
                </div>
                <div class="card-midlle">
                    <h3 class="text d-flex justify-content-center">Call Of Duty</h3>
                    <p class="title d-flex justify-content-center">December 25,2022 4:00 PM</p>
                </div>
                <div class="card-bottom d-flex justify-content-evenly py-4 ">
                    <div class="d-flex align-items-center ">
                        <img src="/img/icon/youtube-icon.png" alt="">
                        <p class="text mt-2">Youtube</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/twitch.png" alt="" class="w-50">
                        <p class="text mt-2 ml-2">Twitch</p>
                    </div>
                </div>
            </div>
            <!-- CARD -->

            <!-- CARD -->
            <div class="card">
                <div class="card-top d-flex justify-content-between py-4 px-4 ">
                    <div><img src="/img/game-img-3.png" alt="">

                    </div>
                    <div><img src="/img/verus-icon.png" alt="">
                    </div>
                    <div><img src="/img/game-img-4.png" alt="">
                    </div>
                </div>
                <div class="card-midlle">
                    <h3 class="text d-flex justify-content-center">Call Of Duty</h3>
                    <p class="title d-flex justify-content-center">December 25,2022 4:00 PM</p>
                </div>
                <div class="card-bottom d-flex justify-content-evenly py-4 ">
                    <div class="d-flex align-items-center ">
                        <img src="/img/icon/youtube-icon.png" alt="">
                        <p class="text mt-2">Youtube</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/twitch.png" alt="" class="w-50">
                        <p class="text mt-2 ml-2">Twitch</p>
                    </div>
                </div>
            </div>
            <!-- CARD -->

            <!-- CARD -->
            <div class="card">
                <div class="card-top d-flex justify-content-between py-4 px-4 ">
                    <div><img src="/img/game-img-5.png" alt="">

                    </div>
                    <div><img src="/img/verus-icon.png" alt="">
                    </div>
                    <div><img src="/img/game-img-6.png" alt="">
                    </div>
                </div>
                <div class="card-midlle">
                    <h3 class="text d-flex justify-content-center">Call Of Duty</h3>
                    <p class="title d-flex justify-content-center">December 25,2022 4:00 PM</p>
                </div>
                <div class="card-bottom d-flex justify-content-evenly py-4 ">
                    <div class="d-flex align-items-center ">
                        <img src="/img/icon/youtube-icon.png" alt="">
                        <p class="text mt-2">Youtube</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/twitch.png" alt="" class="w-50">
                        <p class="text mt-2 ml-2">Twitch</p>
                    </div>
                </div>
            </div>
            <!-- CARD -->

            <!-- CARD -->
            <div class="card">
                <div class="card-top d-flex justify-content-between py-4 px-4 ">
                    <div><img src="/img/game-img-7.png" alt="">

                    </div>
                    <div><img src="/img/verus-icon.png" alt="">
                    </div>
                    <div><img src="/img/game-img-8.png" alt="">
                    </div>
                </div>
                <div class="card-midlle">
                    <h3 class="text d-flex justify-content-center">Call Of Duty</h3>
                    <p class="title d-flex justify-content-center">December 25,2022 4:00 PM</p>
                </div>
                <div class="card-bottom d-flex justify-content-evenly py-4 ">
                    <div class="d-flex align-items-center ">
                        <img src="/img/icon/youtube-icon.png" alt="">
                        <p class="text mt-2">Youtube</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/twitch.png" alt="" class="w-50">
                        <p class="text mt-2 ml-2">Twitch</p>
                    </div>
                </div>
            </div>
            <!-- CARD -->
            <div class="button-icon  ">
                <button class="green-button">VIEW ALL MATCH</button>
            </div>
        </div>

    </div>
</template>

<style lang="scss" scoped>
.wrapper {
    background-color: #212733;
    height: 150vh;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.title {
    color: #93c067;
}

.description,
.text {
    color: white;
}

.container-cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

.card {
    background-color: #28344a;
    border-color: #505e7a;
    width: calc(50% - 10px);
}

.card-midlle {
    background-color: #30415f;
    padding: 20px;
    display: flex;
    flex-direction: column;
}

.button-icon {
    width: 100%;
    display: flex;
    justify-content: center;
    margin: 5rem;


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
