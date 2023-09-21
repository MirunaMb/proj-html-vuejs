<script>
// import MyComponent from "./components/MyComponent.vue";

export default {
    data() {
        return {

        }
    }

    // components: {
    //   MyComponent,
    // },
};
</script>

<template>
    <div class="wrapper">
        <div class="col d-flex flex-column align-items-center ">
            <h3 class="title ">Trending Battle</h3>
            <h1 class="text">Keep Eyes & Manage Upcoming</h1>
            <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi sapiente itaque dicta. Inventore
                explicabo nihil alias ipsum consequuntur facilis cumque.
            </p>
        </div>
        <div class="container-cards d-flex">
            <!-- CARD -->
            <div class="card">
                <div class="card-top d-flex justify-content-between ">
                    <div>
                        <img src="/img/team-players-6.png" alt="" class="image-card">
                    </div>
                </div>
                <div class="card-middle d-flex justify-content-evenly py-4 ">
                    <div class="d-flex align-items-center ">
                        <img src="/img/icon/clock.png" alt="" class="w-25">
                        <p class="title py-2 d-flex align-items-center">10 Min</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/eye.png" alt="" class="w-25">
                        <p class="title mt-2 ml-2">240</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/calendar.png" alt="" class="w-25">
                        <p class="title mt-2 ml-2">Apr 11,2022</p>
                    </div>
                </div>
                <div class="card-bottom">
                    <h3 class="text d-flex justify-content-center">Secrets To An Amazing Role Playing Game</h3>
                </div>

            </div>
            <div class="card">
                <div class="card-top d-flex justify-content-between ">
                    <div>
                        <img src="/img/team-players-7.png" alt="" class="image-card">
                    </div>
                </div>
                <div class="card-middle d-flex justify-content-evenly py-4 ">
                    <div class="d-flex align-items-center ">
                        <img src="/img/icon/clock.png" alt="" class="w-25">
                        <p class="title py-2 d-flex align-items-center">10 Min</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/eye.png" alt="" class="w-25">
                        <p class="title mt-2 ml-2">240</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/calendar.png" alt="" class="w-25">
                        <p class="title mt-2 ml-2">Apr 11,2022</p>
                    </div>
                </div>
                <div class="card-bottom">
                    <h3 class="text d-flex justify-content-center">Secrets To An Amazing Role Playing Game</h3>
                </div>

            </div>
            <div class="card">
                <div class="card-top d-flex justify-content-between ">
                    <div>
                        <img src="/img/team-players-8.png" alt="" class="image-card">
                    </div>
                </div>
                <div class="card-middle d-flex justify-content-evenly py-4 ">
                    <div class="d-flex align-items-center ">
                        <img src="/img/icon/clock.png" alt="" class="w-25">
                        <p class="title py-2 d-flex align-items-center">10 Min</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/eye.png" alt="" class="w-25">
                        <p class="title mt-2 ml-2">240</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/calendar.png" alt="" class="w-25">
                        <p class="title mt-2 ml-2">Apr 11,2022</p>
                    </div>
                </div>
                <div class="card-bottom">
                    <h3 class="text d-flex justify-content-center">Secrets To An Amazing Role Playing Game</h3>
                </div>

            </div>
            <div class="card">
                <div class="card-top d-flex justify-content-between ">
                    <div>
                        <img src="/img/team-players-9.png" alt="" class="image-card">
                    </div>
                </div>
                <div class="card-middle d-flex justify-content-evenly py-4 ">
                    <div class="d-flex align-items-center ">
                        <img src="/img/icon/clock.png" alt="" class="w-25">
                        <p class="title py-2 d-flex align-items-center">10 Min</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/eye.png" alt="" class="w-25">
                        <p class="title mt-2 ml-2">240</p>
                    </div>
                    <div class="d-flex align-items-center">
                        <img src="/img/icon/calendar.png" alt="" class="w-25">
                        <p class="title mt-2 ml-2">Apr 11,2022</p>
                    </div>
                </div>
                <div class="card-bottom">
                    <h3 class="text d-flex justify-content-center">Secrets To An Amazing Role Playing Game</h3>
                </div>

            </div>
            <!-- CARD -->


        </div>
    </div>
</template>

<style lang="scss" scoped>
.wrapper {
    background-color: black;
    height: 100vh;

}

// COLORS
.title {
    color: #93c067;

}

.text {
    color: white;
    padding: 10px;

}

// Cards
.container-cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

.card {
    background-color: #28344a;
    border-color: #505e7a;
    width: 300px;


}

.card-midlle {
    background-color: #30415f;
    padding: 20px;
    display: flex;
    flex-direction: column;
}

.card-top {
    width: 500px;
}

.image-card {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

// cards

// COLORS
</style>