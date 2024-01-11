<template>
  <v-app>
    <HeaderVuetify />
        <v-main>
              <HeroComponent />
              <AboutUs />
              <PortfolioComponent />
              <ProjectComponent />
              <GalleryComponent />
              <ContactUs />
              <FooterComponent />
          </v-main>
  </v-app>
</template>

<script>
import HeaderVuetify from "./components/HeaderVuetify.vue";
import HeroComponent from "./components/HeroComponent.vue";
import AboutUs from "./components/AboutUs.vue";
import PortfolioComponent from "./components/PortfolioComponent.vue";
import ProjectComponent from "./components/ProjectComponent.vue";
import GalleryComponent from "./components/GalleryComponent.vue";
import ContactUs from "./components/ContactUs.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default {
  name: 'App',

  components: {
    HeaderVuetify,
    HeroComponent,
    AboutUs,
    PortfolioComponent,
    ProjectComponent,
    GalleryComponent,
    ContactUs,
    FooterComponent,
  },

  data(){
    return{
        menus:[
          {title:'Home',        route:'home'},
          {title:'About Us',    route:'about-us'},
          {title:'Portfolio',   route:'portfolio'},
          {title:'Project',     route:'project'},
          {title:'Gallery',     route:'galery'},
          {title:'Contact',     route:'contact'},
    ]
    }
},
};
</script>

<style>
  * {
    font-family:'Roboto';
  }
</style>


