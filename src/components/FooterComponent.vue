<template>
    <v-footer padless>
        <v-layout justify-center>
            <v-row justify="center">
                <v-flex xs12 lg12>
                    <v-toolbar-title class="text-center mt-10">Web Burden</v-toolbar-title>
                        <v-layout column >
                            <v-card-text xs12 lg12 class="text-center pt-8 d-flex justify-center icons">
                                <router-link>
                                    <v-icon large>mdi-github</v-icon>
                                </router-link>

                                <router-link to="/linkedin">
                                    <v-icon large>mdi-linkedin</v-icon>
                                </router-link>

                                <router-link to="/instagram">
                                    <v-icon large>mdi-instagram</v-icon>
                                </router-link>

                                <router-link to="/facebook">
                                    <v-icon large>mdi-facebook</v-icon>
                                </router-link></v-card-text>

                                </v-layout>
                                    <v-subheader class="text-center pt-10">
                                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni quidem autem accusamus ratione nulla, totam libero? Quaerat necessitatibus alias ipsum iure fugit in mollitia eveniet itaque? Praesentium officiis laboriosam deserunt!
                                    </v-subheader>
                                        <v-layout align-content-center justify-center>
                                            <v-form class="mt-10">
                                                <v-text-field class="mt-5" label="Email" outlined dense />
                                                    <v-btn block rounded color="success">Subscribe Us</v-btn>
                                            </v-form>
                                        </v-layout>
                                    </v-flex>
                                    <div class="mt-10">
                                        <v-divider></v-divider>
                                        <v-subheader class="pb-7">
                                            © Copyright Web Burden. All Rights Reserved - <strong>Vuetify 2023</strong>
                                        <v-spacer />
                                        </v-subheader>
                                    </div>
                                </v-row>
                            </v-layout>
                        <v-card
                                flat
                                tile
                                class="indigo lighten-1 white--text text-center"
                            >

                            <v-card-text class="white--text pt-2">
                                Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet dui. Duis commodo vitae velit et faucibus. Morbi vehicula lacinia malesuada. Nulla placerat augue vel ipsum ultrices, cursus iaculis dui sollicitudin. Vestibulum eu ipsum vel diam elementum tempor vel ut orci. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
                            </v-card-text>
                        <v-divider></v-divider>
                </v-card>
        </v-footer>
</template>

<script>
    export default {
        name: 'FooterComponent.vue',
    }
</script>