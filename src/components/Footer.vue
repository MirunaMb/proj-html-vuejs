<script>
export default {
    data() {
        return {
            send: '',
            images: [
                { image: '/img/icon/youtube.png' },
                { image: '/img/icon/twitch.png' },
                { image: '/img/icon/youtube-icon.png' },
                { image: '/img/icon/twitch-icon.png' },

            ],
            links: [
                { text: 'Quick Links', url: 'link_a' },
                { text: 'Games', url: 'link_b' },
                { text: 'Latest Tournament', url: 'link_c' },
                { text: 'Shop', url: 'link_d' },
                { text: 'Blog', url: 'link_e' },
                { text: 'Videos', url: 'link_f' },
                { text: 'Contact', url: 'link_g' },
            ],
            faqs: [
                { text: 'Help', url: 'link_h' },
                { text: 'Faqs', url: 'link_i' },
                { text: 'Term & Conditions', url: 'link_j' },
                { text: 'Privacy', url: 'link_j' },
            ],
            follows: [
                { text: 'Follow Us', url: 'link_k' },
                { text: 'Facebook', url: 'link_k' },
                { text: 'Twitter', url: 'link_l' },
                { text: 'Instagram', url: 'link_m' },
                { text: 'Youtube', url: 'link_n' },
                { text: 'Github', url: 'link_o' },
            ],
            contacts: [
                { text: 'Location:', url: 'link_v' },
                { text: '4 Mayfield,Buckden,PE19 5SZ', url: 'link_v' },
                { text: 'Phone:', url: 'link_w' },
                { text: '(302)555-0107', url: 'link_x' },
            ],

        };
    },
    methods: {
        sendEmail() {
            const emailAddress = this.send;
            if (!emailAddress || emailAddress.trim() === '') {
                alert('Inserisci un indirizzo email valido.');
                return;
            }
            alert('Email inviata a: ' + this.send);
        },
    },
};
</script>


<template>
    <div class="wrapper">
        <div class="footer-top">
            <div class="subscribe-text">
                <h1>Subscribe Newsletter</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis, laudantium?</p>
            </div>
            <!-- CONTAINER FORM -->
            <div class="container-form">
                <form class="d-flex" role="send">
                    <input v-model="send" class="form-control" type="text" placeholder="Enter your email" aria-label="Send">
                    <img src="/img/icon/send-icon.png" alt="" class="image-form" @click="sendEmail">
                </form>
            </div>
            <!-- CONTAINER FORM -->
        </div>
        <div class="footer-midlle">
            <div class="logo-footer">
                <img src="/img/logo.png" alt="" class="w-25">
                <p class="text py-2">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Doloremque, ipsum.
                </p>
            </div>
            <div class="pics">
                <ul>
                    <li v-for="image in images">
                        <img :src="image.image" class="image-footer" />
                    </li>
                </ul>
            </div>
            <div class="menu-footer">
                <ul>
                    <li v-for="(item, index) in links" :key="index" :class="(index == 0) ? 'first-item' : ''">
                        <a href="links.url">{{ item.text }}</a>
                    </li>
                </ul>
                <ul>
                    <li v-for="(item, index) in faqs" :key="index" :class="(index == 0) ? 'first-item' : ''">
                        <a href="faqs.url">{{ item.text }}</a>
                    </li>
                </ul>
                <ul>
                    <li v-for="(item, index) in follows" :key="index" :class="(index == 0) ? 'first-item' : ''">
                        <a href="follows.url">{{ item.text }}</a>
                    </li>
                </ul>
                <ul>
                    <li v-for="(item, index) in contacts" :key="index" :class="(index == 0) ? 'first-item' : ''">
                        <a href="contacts.url">{{ item.text }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
    <div class="wrapper-footer">
        <div class="footer-bottom">
            <p class="white-text">Copyright © 2022
                <span class="green-text">FUTIO.</span>
                All rights reserved.
            </p>
        </div>
    </div>
</template>
  

<style lang="scss" scoped>
.wrapper {
    height: 75vh;
    background-color: #28344a;
    position: relative;
}

.footer-top {
    width: 80%;
    height: 300px;
    background-color: #30415f;
    display: flex;
    border-radius: 50px;
    position: absolute;
    top: -15%;
    left: 10%;

}

.subscribe-text {
    color: #faf7f8;
    padding: 40px;
    width: 600px;
    height: 300px;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
}

// Form
.container-form {
    height: 300px;
    display: flex;
    align-items: center;
}


.form-control {
    width: 400px;
    height: 50px;
    background-color: #435374;
    border-color: #516588;
}

.image-form {
    width: 50px;
    height: 50px;
    background-color: #93cb50;
    border-radius: 25px;
    margin-left: -40px;
}

// Form

// FOOTER MIDLLE
.footer-midlle {
    width: 100%;
    position: absolute;
    top: 300px;
    margin-left: 200px;
}

.logo-footer {
    width: 500px;
}

.text {
    color: #faf7f8;
}

.image-footer {
    width: 1.5rem;
}

.menu-footer {
    display: flex;
    flex-direction: column;
    align-items: center;
    flex-direction: row;
    justify-content: center;
    margin-top: -200px;
}

.pics {
    width: 200px;
}

.pics ul {
    display: flex;
}

ul {
    list-style: none;
    width: 200px;

}

a {
    text-decoration: none;
    color: #999a9c;
}

li {
    padding: 10px;
}

li.first-item a {
    color: white;
}

.wrapper-footer {
    height: 100px;
    background-color: #1b212d;
}

.footer-bottom {
    display: flex;
    justify-content: center;
}

.white-text {
    color: #c2c6ce;
}

.green-text {
    color: #788d68;
}
</style>