<template>
    <div>
        <div class="bg">
            <video muted autoplay loop playsinline src="video/market.mp4"></video>
            <div class="text">
                <h1><span class="chromeColor">Bullseye</span> for Chrome</h1>
                <p>Groceries Made Easy</p>
                <br />
                <center>
                    <v-btn @click="moveAbout()" class="learnMoreButton" elevation="3" height="48px" color="white">Learn
                        More</v-btn>
                </center>
                <br />
                <br />
                <br />
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: "LandingPage",

    components: {
    },

    data: () => ({

    }),

    methods: {
        moveAbout() {
            this.$router.push({
                path: "about"
            });
        },
        moveContact() {
            this.$router.push({
                path: "contact",
            });
        },
        moveHome() {
            this.$router.push({
                path: "/",
            });
        },

    },
};
</script>

<style scoped>
.chromeColor {
    color: red;
}

.bg {
    width: 100%;
    height: 100%;
    overflow: hidden;
    margin: 0px auto;
    position: relative;
}

video {
    width: 100%;
    height: 100%;
}

.text {
    position: absolute;
    width: 100%;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.text h1 {
    text-align: center;
    font-family: Georgia, 'Times New Roman', Times, serif;
    font-size: 46px;
    color: #ffffff;
}

.text p {
    font-family: Georgia, 'Times New Roman', Times, serif;
    font-style: italic;
    text-align: center;
    font-weight: bold;
    font-size: 31px;
    color: #ffffff;
}


/*------------------*/
/* Layout (No Edit) */
/*------------------*/
@media screen and (max-width: 600px) {
    .bg {
        width: 100%;
        height: 100%;
    }

    .text {
        position: absolute;
        width: 100%;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    .text h1 {
        text-align: center;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 20px;
        color: #ffffff;
    }
    
    .text p {
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-style: italic;
        text-align: center;
        font-weight: bold;
        font-size: 20px;
        color: #ffffff;
    }

}

.name {
    text-align: center;
    font-family: 'Times New Roman', Times, serif;
    font-size: 43px;
    font-weight: bold;
    font-style: italic;
    margin-bottom: 15px;
    color: white;
}

.learnMoreButton {

    font-weight: bold;
}

.imageText {
    text-align: center;
    font-family: 'Times New Roman', Times, serif;
    font-size: 35px;
    font-weight: bold;
    color: white;
}

@media screen and (max-width: 600px) {
    .imageText {
        font-size: 30px;
    }
}

.wrapper {
    display: grid;
    place-items: center;
    min-height: 70vh;
}

.content {
    font-family: system-ui, serif;
    font-size: 1.5rem;
    padding: 2rem;
    border-radius: 1rem;
}
</style>
