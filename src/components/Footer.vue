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
        <div class="footer-top">
            <div class="subscribe-text">
                <h1>Subscribe Newsletter</h1>
                <p class="py-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis, laudantium?</p>
            </div>
        </div>
        <div class="footer-midlle">middle</div>
        <div class="footer-bottom">bottom</div>
    </div>
</template>

<style lang="scss" scoped>
.wrapper {
    height: 100vh;
    background-color: #28344a;
}

.footer-top {
    width: 80%;
    height: 300px;
    background-color: #30415f;
    display: flex;
    border-radius: 50px;
}

.subscribe-text {
    color: #faf7f8;
    padding: 40px;
    width: 600px;
}
</style>