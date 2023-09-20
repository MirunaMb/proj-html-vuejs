<script>
// import MyComponent from "./components/MyComponent.vue";

export default {
    data() {
        return {
            title: "Hello world"
        }
    }

    // components: {
    //   MyComponent,
    // },
};
</script>

<template>
    <div class="wrapper">
        <div class="d-flex flex-column align-items-center py-5">
            <h1 class="text">Futio Quick Facts</h1>
        </div>
        <div class="container-cards d-flex justify-content-between py-4 px-4">
            <div class="card">
                <div class="py-5 px-5">
                    <div class="number">1135</div>
                    <div class="title ms-4">Twitch Streams</div>
                </div>

            </div>
            <div class="card">
                <div class="py-5 px-5">
                    <div class="number ms-5">44</div>
                    <div class="title ms-5">Total Games</div>
                </div>

            </div>
            <div class="card">
                <div class="py-5 px-5">
                    <div class="number ms-4">982</div>
                    <div class="title ms-4">Youtube Streams</div>
                </div>

            </div>
            <div class="card">
                <div class="py-5 px-5">
                    <div class="number ms-5">40</div>
                    <div class="title ms-5">Pro Team</div>
                </div>

            </div>

        </div>
    </div>
</template>

<style lang="scss" scoped>
.wrapper {
    background-color: #000000;
    height: 50vh;

}

.text {
    color: white;
    font-size: 70px;

}

.title {
    color: #93c067;
}

.card {
    width: 300px;
    height: 200px;
    border-color: #151517;
    background-color: #000;
    border-radius: 50px;
}

.number {
    color: white;
    font-size: 70px;
}
</style>