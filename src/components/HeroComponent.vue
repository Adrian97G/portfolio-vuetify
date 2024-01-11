<template>
    <v-container class="pt-3 mt-10">
        <v-layout d-flex flex-column flex-md-row justify-space-between align-center pointer>
            <v-flex xs12 text-center>
                <h2 class="intro-text">Welcome to our Vuetify App</h2>
                <p class="description" >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Optio numquam laudantium, autem praesentium, voluptate possimus fugiat harum iste.</p>
                <v-btn color="success" class="white--text mr-10" rounded>Get Started</v-btn>
                <v-btn color="indigo" class="white--text" rounded>
                    <v-icon>mdi-play-circle</v-icon> Watch Video
                </v-btn>
            </v-flex>
            <v-flex xs12 lg6>
                <img width="100%" src="@/assets/Images/hero.svg" alt="Hero Image" />
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
    export default {
        name: "HeroComponent",
    }

</script>

<style scoped>
    h2.intro-text {
        font-size: 40px;
        font-weight: bold;
        color: #444;
    }

    p.description {
        font-size: 20px;
        margin: 20px 0px;
        color: #444444ba;
    }

</style>