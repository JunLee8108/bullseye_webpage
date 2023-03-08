<template>
    <div>
        <v-btn class="name" height="50px" width="100%" @click="moveHome()" block color="black" :class="{ 'on-hover': hover }"
            :elevation="hover ? 5 : 0">
            Home
        </v-btn>
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
.name {
    text-align: center;
    margin-right: 15px;
}

@media screen and (max-width: 600px) {
    .name {
        font-size: 13px;
        margin-right: 5px;
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
