<template>
    <div>
        <NavigationVue />
        <div class="firstBox">
            <div class="wrapper">
                <img src="img/Bullseye.png" height="400px">
            </div>
            <div class="secondBox">
                <div class="intro">
                    bbasdasdasdasddas
                </div>
                
            </div>
        </div>






    </div>
</template>

<script>
import NavigationVue from './Navigation.vue';

export default {
    name: "AboutPage",

    components: {
        NavigationVue,
    },

    data: () => ({

    }),

    methods: {
        moveAbout() {
            this.$router.push({
                path: "about",
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
.firstBox {
    width: 100%;
    height: 500px;
}

.secondBox {
    background-color: white;
    width: 100%;
    height: 499px;
}

.wrapper {
    position: absolute;
    width: 50%;
    top: 5%;
    left: 20%;
}

.intro {
    position: absolute;
    left: 50%;
    top: 30%;
}

.name {
    text-align: center;
    font-family: 'Times New Roman', Times, serif;
    font-size: 23px;
    font-weight: bold;
    font-style: italic;
    margin-bottom: 15px;
    color: white;
}

.learnMoreButton {
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-weight: bold;
}

.imageText {
    text-align: center;
    font-family: 'Times New Roman', Times, serif;
    font-size: 40px;
    font-weight: bold;
    color: white;
}

@media screen and (max-width: 600px) {
    .imageText {
        font-size: 30px;
    }
}



.content {
    font-family: system-ui, serif;
    font-size: 1.5rem;
    padding: 2rem;
    border-radius: 1rem;
}
</style>
