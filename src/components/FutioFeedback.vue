<script>
export default {
    data() {
        return {
            reviews: [
                {
                    stars: 5,
                    text: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sequi necessitatibus minima aut fuga. ",
                    userImage: "/img/testimonials-image-1.png",
                    userName: "Kiribati",
                    userCountry: "Italia",
                },
                {
                    stars: 4,
                    text: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sequi necessitatibus minima aut fuga. ",
                    userImage: "/img/testimonials-image-2.png",
                    userName: "Kiribati",
                    userCountry: "USA",
                },
                {
                    stars: 5,
                    text: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sequi necessitatibus minima aut fuga. ",
                    userImage: "/img/testimonials-image-3.png",
                    userName: "Kim",
                    userCountry: "Italia",
                },
                {
                    stars: 5,
                    text: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sequi necessitatibus minima aut fuga. ",
                    userImage: "/img/testimonials-image-2.png",
                    userName: "Kiribati",
                    userCountry: "Usa",
                },
                {
                    stars: 5,
                    text: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sequi necessitatibus minima aut fuga. ",
                    userImage: "/img/testimonials-image-3.png",
                    userName: "Alice",
                    userCountry: "France",
                },
            ],
        };
    },
};
</script>

<template>
    <div class="wrapper">
        <div class="col d-flex flex-column align-items-center py-5">
            <h3 class="title">Trending Battle</h3>
            <h1 class="text">Keep Eyes & Manage Upcoming</h1>
            <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi sapiente itaque dicta. Inventore
                explicabo nihil alias ipsum consequuntur facilis cumque.</p>
        </div>

        <!-- Carosello delle recensioni -->
        <div class="reviews-carousel">
            <div class="carousel">
                <div class="review-card" v-for="(review, index) in reviews" :key="index">
                    <div class="stars">
                        <!-- Aggiungi stili alle stelle qui -->
                    </div>
                    <p class="review-text">{{ review.text }}</p>
                    <div class="user-info">
                        <img :src="review.userImage" alt="User Image" class="user-image" />
                        <p class="user-name">{{ review.userName }}</p>
                        <p class="user-country">{{ review.userCountry }}</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="offer-container">
            <div>
                <img src="/img/banner-item-obj1.png" alt="" class="phone">
            </div>
            <div class="text-offer">
                <h3>Make Offer</h3>
                <h1 class="text-discount">Get 70% Offer Discount</h1>
                <button class="green-button">
                    <p class="ms-4 px-3">Get Offers</p>
                </button>
            </div>

            <div>
                <img src="/img/banner-item-obj2.png" alt="" class="headphones">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.wrapper {
    background-color: #000000;
    height: 150vh;
    position: relative;
}

/* COLORS */
.title {
    color: #93c067;
}

.text {
    color: white;
}

// Carousel 
.reviews-carousel {
    display: flex;
    justify-content: center;
    overflow: hidden;
    width: 100%;
    margin-top: 20px;
}

.carousel {
    display: flex;
    animation: scroll 20s linear infinite;
}

.review-card {
    margin-right: 20px;
    flex: 0 0 auto;
    background-color: #28344a;
    padding: 20px;
    border-radius: 10px;
    text-align: center;
    width: 300px;
}

.review-text {
    margin-top: 10px;
    color: white;
}

.user-info {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 10px;
}

.user-image {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    margin-right: 10px;
    color: white;
}

.user-name {
    color: white;
}

.user-country {
    line-height: 20px;
    margin-left: 5px;
    color: #6e8a68;
}

// MAKE AN OFFER SECTION 
.offer-container {
    width: 100%;
    height: 75vh;
    background-image: url('/img/banner-item-bg.png');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    position: relative;
    padding: 20px;
    display: flex;
    justify-content: center;
    justify-content: space-between;
    margin-top: 200px;
}

.phone {
    width: 300px;
}

.text-offer {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 200px;
    color: white;

}

.text-discount {
    font-size: 3.5rem;
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

.headphones {
    width: 300px;

}

// MAKE AN OFFER SECTION
</style>
