<template>
    <v-app-bar
            style="padding: 0px 90px"
            app
            color="white"
            lightelevation="0"
            >
            <v-flex xs-6 justify-center>
                <v-toolbar-title class="text-center">AdrianDev</v-toolbar-title>
            </v-flex>
            <v-spacer />

              <!-- Botón del menú para dispositivos móviles -->
              <v-btn icon @click.stop="toggleDrawer" class="d-lg-none">
                    <v-icon large right text-center class="mt-2">mdi-menu</v-icon>
              </v-btn>

              <!-- Lista de navegación para pantallas grandes (lg y superior) -->
              <v-list class="d-none d-lg-flex">
                    <v-list-item v-for="(menu, index) in menus" :key="index">
                      <router-link :to="menu.route">
                        <v-list-item-title>{{ menu.title }}</v-list-item-title>
                      </router-link>
                    </v-list-item>

                    <!-- Otros elementos del menú -->

                  </v-list>

                  <!-- Contenido de la aplicación -->
                  <v-main>
                    <router-view></router-view>
                  </v-main>
                  <v-navigation-drawer app v-model="drawer" mobile class="navigation-drawer">
                    <v-list>
                      <v-list-item v-for="(menu, index) in menus" :key="index" class="navigation-drawer-item">
                        <router-link :to="menu.route">
                          <v-list-item-title>{{ menu.title }}</v-list-item-title>
                        </router-link>
                      </v-list-item>
                      <v-btn text>
                          <v-icon>mdi-magnify</v-icon>
                      </v-btn>
                  <v-btn outlined color="success">Get Started</v-btn>
            </v-list>
        </v-navigation-drawer>
    </v-app-bar>
</template>

  <script>
  export default {
    name: "HeaderVuetify",
    data() {
      return {
        drawer: false,
        menus: [
            { title: 'Hero', route: '/hero' },
            { title: 'About Us', route: '/about-us' },
            { title: 'Portfolio', route: '/portfolio' },
            { title: 'Project', route: '/project' },
            { title: 'Gallery', route: '/gallery' },
            { title: 'Contact', route: '/contact' },
        ],
      };
    },
    methods: {
      toggleDrawer() {
        this.drawer = !this.drawer;
      },
    },
  };
  </script>

  <style>
  .v-toolbar__title {
    font-size: 32px;
    color: #4caf50;
    font-weight: 700;
  }

  .navigation-drawer {
    background-color: #4caf50;
    color: #000;
    font-weight: 500;
    opacity: 1;
  }

  .navigation-drawer-item:hover {
    background-color: #388e3c;
    transition: background-color 0.3s;
    transform: scale(1);
  }

  .navigation-drawer a {
    text-decoration: none;
    color: inherit;
  }
  </style>
