<template>
    <v-container fluid grid-list-md>
        <v-layout row wrap>
            <v-flex xs12 sm6 md12 text-center>
                <v-subheader class="text-h4 justify-center">Contact Us</v-subheader>
                    <p>
                        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quidem,
                        quaerat nobis! Earum placeat necessitatibus.
                    <br />
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Impedit, deserunt eos iure, expedita blanditiis architecto quas sunt quisquam, repellendus fuga optio vero quibusdam quidem aut dolor! Fuga facere nostrum laudantium.
                    </p>
            </v-flex>
            <v-flex d-flex xs12 sm6 md6>
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d16290448.735104078!2d-85.02140224367125!3d4.5651834912836335!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8e15a43aae1594a3%3A0x9a0d9a04eff2a340!2sColombia!5e0!3m2!1ses-419!2sco!4v1704755797692!5m2!1ses-419!2sco" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </v-flex>
            <v-col>
            <v-flex>
                <form ref="form">
                    <v-form ref="form">
                        <v-text-field
                                label="Name"
                                required
                            >
                            </v-text-field>

                            <v-select
                                label="Item"
                                required
                            >
                            </v-select>

                            <v-checkbox
                                v-model="checkbox"
                                label="Do you agree?"
                                required
                            >
                            </v-checkbox>

                            <div class="d-flex flex-column">
                                <v-btn
                                    color="success"
                                    class="mt-4"
                                    block
                                >
                                    Send
                                </v-btn>

                                <v-btn
                                    color="error"
                                    class="mt-4"
                                    block
                                >
                                    Reset Form
                                </v-btn>
                            </div>



                    </v-form>
                    </form>
            </v-flex>
        </v-col>
    </v-layout>
</v-container>
</template>

<script>
    export default {
        name: 'ContactUs',
    }

</script>
