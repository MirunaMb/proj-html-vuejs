

<template>
    <div class="wrapper">
        <div>
            <img src="img/live-streaming-bg.png" alt="">
        </div>
        <div class="col d-flex flex-column align-items-center py-5">
            <h3 class="title ">Trending Battle</h3>
            <h1 class="text">Keep Eyes & Manage Upcoming</h1>
            <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi sapiente itaque dicta. Inventore
                explicabo nihil alias ipsum consequuntur facilis cumque.
            </p>
        </div>
        <div class="col-image ">
            <img src="img/stream-bg-3.png" alt="" class="stream-image">
            <div class="container-button">
                <button type="button" class="btn btn-warning">
                    <img src="/img/icon/live-icon.png" alt="" class="image-live">
                    <p class="live-text">Live</p>
                </button>
            </div>
            <div class="containe-play">
                <div class="play-button">
                    <img src="/img/icon/play-icon.png" alt="Play">
                </div>
                <h3>League Of Legends</h3>
            </div>
            <div class="viewers d-flex">
                <p class="title ">356,599 </p>
                <p class="ms-3">Viewers</p>
                <p class="title ms-3">23,599 </p>
                <p class="ms-3">Likes</p>
            </div>


        </div>
    </div>
</template>

<style lang="scss" scoped>
.wrapper {
    background-color: #000000;
    height: 100vh;
    position: relative;

}

// COLORS
.title {
    color: #93c067;
}

.text {
    color: white;
}

// COLORS

// CONTAINER & IMAGE 
.col {
    position: absolute;
    bottom: 800px;
    left: 50px;
}

.col-image {
    width: 80%;
    height: 50vh;
    position: relative;

}

.stream-image {
    width: 100%;
    height: 100%;
    position: absolute;
    bottom: 200px;
    left: 150px;
    filter: blur(2px);


}

// CONTAINER & IMAGE 

// BUTTON LIVE
.container-button {
    position: relative;
}

.btn-warning {
    width: 110px;
    height: 50px;
    border-radius: 20px;
    display: flex;
    position: absolute;
    right: -90px;
    bottom: 110px;
}

.image-live {
    width: 25px;
    object-fit: contain;
}

.live-text {
    line-height: 30px;
    margin-top: 5px;
    margin-left: 15px;
}

// BUTTON LIVE

// Button Play
.play-button {
    display: inline-block;
    width: 64px;
    height: 60px;
    border: 4px solid #ccc;
    border-radius: 50%;
    background-color: white;
    text-align: center;
    line-height: 64px;
    position: absolute;
    left: 60%;
    top: 10%;

}

.play-button img {
    width: 30%;
    height: auto;
    margin-bottom: 15px;
}

.containe-play {
    position: relative;
}

.containe-play h3 {
    position: absolute;
    bottom: 50%;
    left: 54%;
    color: white;
}

.viewers {
    position: absolute;
    bottom: 200px;
    left: 200px;
    color: white;
    margin: 10px;
}

.viewers p {}




// Button Play
</style>