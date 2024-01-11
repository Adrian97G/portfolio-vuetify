<template>
    <v-container>
      <v-row align="center" justify="center">
        <v-col lg="6" md="6" sm="12">
          <img src="@/assets/Images/section-image.svg" alt="Section Img" class="responsive-image" />
        </v-col>
        <v-col lg="6" md="6" sm="12" class="text-center">
              <v-subheader class="text-h4 mt-5 mb-4 justify-center">About Us</v-subheader>
              <p class="body-1">
                Nihil quis obcaecati, eaque necessitatibus excepturi quos illo. Unde dolorem corporis cumque fugiat nobis sequi
                necessitatibus nulla natus non quibusdam, esse quidem!
              </p>
          <v-list>
            <v-list-item v-for="(item, index) in items" :key="index">
              <v-list-item-icon>
                <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
                <v-list-item-subtitle>{{ item }}</v-list-item-subtitle>
              </v-list-item-icon>
            </v-list-item>
          </v-list>
          <p class="mt-5">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo suscipit consequuntur aspernatur eius sapiente sed,
            error adipisci nam, dolores aut, ratione nobis accusantium veniam cum laborum necessitatibus incidunt consequatur
            ducimus.
          </p>
        </v-col>
      </v-row>
    </v-container>
  </template>

  <script>
  export default {
    name: "AboutUs",
    data() {
      return {
        items: [
          "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptates non fuga quis.",
          "Lorem, ipsum dolor sit amet consectetur adipisicing elit.",
          "Lorem, ipsum dolor sit amet consectetur adipisicing elit."
        ]
      };
    }
  };
</script>


