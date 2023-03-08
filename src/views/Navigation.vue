<template>
    <div>
        <v-app-bar app elevation="0" color="#8B0000" height="70px">
            <v-spacer></v-spacer>
            <v-btn class="name" @click="moveHome()" text height="70px" color="#808080">
                <div class="font">
                    Home
                </div>
            </v-btn>
            <v-btn class="name" @click="moveAbout()" text height="70px" color="#808080">
                <div class="font">
                    About Us
                </div>
            </v-btn>
            <v-spacer></v-spacer>
        </v-app-bar>
        <v-divider></v-divider>
        <!-- <v-toolbar flat height="72">
            <v-switch
              v-model="$vuetify.theme.dark"
              inset
              label="Vuetify Theme Dark"
            ></v-switch>
          </v-toolbar> -->
    </div>
</template>

<script>
export default {
    name: "NavigationVue",

    data: () => ({

    }),

    methods: {
        moveAbout() {
            this.$router.push({
                path: "about",
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
.font {
    color: white;
}

.name {
    text-align: center;
    margin-right: 15px;
    color: white;
}

@media screen and (max-width: 600px) {
    .name {
        font-size: 13px;
        margin-right: 5px;
        color: white;
    }
}

.name2 {
    text-align: center;
    margin-left: -10px;
    margin-right: 15px;
}

@media screen and (max-width: 600px) {
    .name2 {
        font-size: 13px;
        margin-right: 5px;
        margin-left: -5px;
    }
}
</style>
