<template>
    <v-container class="my-15">
        <v-layout column>
            <v-flex xs12 lg12>
                <v-subheader class="text-h4 justify-center">Gallery</v-subheader>
                    <p class="text-center">
                        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quidem,
                        quaerat nobis! Earum placeat necessitatibus.

                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat temporibus debitis veniam architecto nesciunt odit aliquam totam dolor inventore porro quo ut sit quis, modi, molestias voluptatem at! Recusandae, laborum!
                    </p>
            </v-flex>
            <v-row>
            <v-col
                v-for="n in 9"
                :key="n"
                class="d-flex child-flex"
                cols="4"
                >
                <v-img
                    :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
                    :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
                    aspect-ratio="1"
                    cover
                class="bg-grey-lighten-2"
            >
                <template v-slot:placeholder>
                <v-row
                    class="fill-height ma-0"
                    align="center"
                    justify="center"
                >
                    <v-progress-circular
                    indeterminate
                    color="grey-lighten-5"
                    ></v-progress-circular>
                </v-row>
                </template>
            </v-img>
            </v-col>
        </v-row>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    name: "GalleryComponent",
}
</script>
