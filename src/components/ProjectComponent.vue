<template>
    <v-container class="my-15">
        <v-row class="justify-center">
            <v-flex justify-center>
                <v-subheader class="text-h4 mb-4 justify-center">Project</v-subheader>
                <p class="text-center">
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quidem,
                    quaerat nobis! Earum placeat necessitatibus, provident nulla totam
                    officiis voluptatum reprehenderit.
                <br />
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur eius et labore nesciunt modi in iure, neque, maxime quis iste inventore fugiat reiciendis provident minus culpa quidem obcaecati minima explicabo!
                </p>
                </v-flex>
                    <v-flex flex-md-row align-self-center align-self-start>
                        <v-card class="mx-auto my-12" max-width="374">
                        <template v-slot:loader="{ isActive }">
                <v-progress-linear
                :active="isActive"
                color="deep-purple"
                height="4"
                indeterminate
                ></v-progress-linear>
                </template>

                <v-img
                    cover
                    height="250"
                    src="https://img.freepik.com/vector-premium/aplicacion-movil-codificacion-concepto-desarrollo-web-programacion-diseno-diseno-receptivo_90099-867.jpg?w=740"
                >
                </v-img>

                <v-card-item>
                <v-card-title>Web Development</v-card-title>

                <v-card-subtitle>
                <span class="me-1">Frontend Development</span>

                <v-icon color="error" icon="mdi-fire-circle" size="small"></v-icon>
                </v-card-subtitle>
                </v-card-item>

                <v-divider class="mx-4"></v-divider>
                <v-card-actions>
                <v-btn color="success" rounded>
                View Details
                </v-btn>
                <v-spacer />
                <v-rating
                    :value="4.5"
                    color="amber"
                    dense
                    half-increments
                    readonlysize="14"
                >
                </v-rating>
                </v-card-actions>
                </v-card>
                </v-flex>
                <v-flex flex-md-row align-self-center align-self-start>
                <v-card class="mx-auto my-12" max-width="374">
                <template v-slot:loader="{ isActive }">
                <v-progress-linear
                :active="isActive"
                color="deep-purple"
                height="4"
                indeterminate
                ></v-progress-linear>
                </template>

                <v-img
                    cover
                    height="250"
                    src="https://img.freepik.com/vector-gratis/coleccion-diseno-sitios-web-receptivos-realistas_23-2149500084.jpg?w=740&t=st=1704832930~exp=1704833530~hmac=fbab8542967bb604e1b6eabe5d48d96f011365b62e76e646501ee18218617b4b"
                >
                </v-img>

                <v-card-item>
                <v-card-title>Web Development</v-card-title>

                <v-card-subtitle>
                <span class="me-1">Frontend Development</span>

                <v-icon color="error" icon="mdi-fire-circle" size="small"></v-icon>
                </v-card-subtitle>
                </v-card-item>

                <v-divider class="mx-4"></v-divider>
                <v-card-actions>
                <v-btn color="success" rounded>
                View Details
                </v-btn>
                <v-spacer />
                <v-rating
                    :value="4.5"
                    color="amber"
                    dense
                    half-increments
                    readonlysize="14"
                >
                </v-rating>
            </v-card-actions>
            </v-card>
            </v-flex>
            <v-col>
                <v-card class="mx-auto my-12" max-width="374">
            <template v-slot:loader="{ isActive }">
                <v-progress-linear
                :active="isActive"
                color="deep-purple"
                height="4"
                indeterminate
                ></v-progress-linear>
            </template>

            <v-img
                cover
                height="250"
                src="https://img.freepik.com/vector-gratis/ilustracion-concepto-diagrama-flujo-usuarios_114360-1658.jpg?t=st=1704753507~exp=1704754107~hmac=d3ce4cf1a7d631cc7a41b533d358c6f352d52cbe05a7ef18f002529b3fee70a6"
            ></v-img>

            <v-card-item>
                <v-card-title>Web Development</v-card-title>

                <v-card-subtitle>
                <span class="me-1">Frontend Development</span>

                <v-icon color="error" icon="mdi-fire-circle" size="small"></v-icon>
                </v-card-subtitle>
            </v-card-item>

            <v-divider class="mx-4"></v-divider>
            <v-card-actions>
                <v-btn color="success" rounded>
                View Details
                </v-btn>
                <v-spacer />
                <v-rating
                    :value="4.5"
                    color="amber"
                    dense
                    half-increments
                    readonlysize="14"
                >
                </v-rating>
            </v-card-actions>
            </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
    export default {
    name: "ProjectComponent",
};
</script>
