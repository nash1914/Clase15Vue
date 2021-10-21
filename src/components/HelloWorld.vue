<template>
  <v-container>
    <v-row class="text-center">
      <!-- <v-col cols="12">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="200"
        />
      </v-col> -->


      <!-- carruzell -->
        <v-carousel>
          <v-carousel-item
            v-for="(item,i) in items"
            :key="i"
            :src="item.src"
            reverse-transition="fade-transition"
            transition="fade-transition"
          ></v-carousel-item>
        </v-carousel>

      <!--Fin Carruzel  -->


      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to Hell
        </h1>

        <p class="subheading font-weight-regular">
          For help and collaboration with other Vuetify developers,
          <br>please join our online
          <a
            href="https://community.vuetifyjs.com"
            target="_blank"
          >Discord Community</a>
        </p>
      </v-col>


      <!-- <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          What's next?
        </h2>

         <v-row justify="center">
          <a
            v-for="(next, i) in whatsNext"
            :key="i"
            :href="next.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ next.text }}
          </a>
   
       </v-col>

       <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          Important Links
        </h2>

        <v-row justify="center">
          <a
            v-for="(link, i) in importantLinks"
            :key="i"
            :href="link.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ link.text }}
          </a>
        </v-row> -->
      <!-- </v-col> -->

      <!-- <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          Ecosystem
        </h2>

        <v-row justify="center">
          <a
            v-for="(eco, i) in ecosystem"
            :key="i"
            :href="eco.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ eco.text }}
          </a>
        </v-row>
      </v-col> -->
    </v-row>

    <!-- inicio Footer -->

    <v-footer padless>
    <v-col
      class="text-center"
      cols="12"
    >
      {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
        </v-col>
  </v-footer>


      <!-- Final Footer -->
  </v-container>

</template>

<script>
  export default {
    name: 'HelloWorld',
 
      data () {
      return {
        items: [
          {
            src: 'https://i.ibb.co/1dJr7gL/halo-infinite-1280x500-xtrafondos-com.jpg',
          },
          {
            src: 'https://i.ibb.co/gtmn5v0/the-legend-of-zelda-breath-of-the-wild-1280x500-xtrafondos-com.jpg',
          },
          {
            src: 'https://i.ibb.co/GtmkLsT/nier-automata-cosplay-1280x500-xtrafondos-com.jpg',
          },
          {
            src: 'https://i.ibb.co/xCJzq7F/personajes-tales-of-arise-1280x500-xtrafondos-com.jpg',
          },
           {
            src: 'https://i.ibb.co/s66s31m/personajes-de-god-of-war-ragnrok-1280x500-xtrafondos-com.jpg',
          },
        ],
      }
    },
  }
  
      // Inicio Script para Footer
      

    // Final Script Footer

    // data: () => ({
    //   ecosystem: [
    //     {
    //       text: 'vuetify-loader',
    //       href: 'https://github.com/vuetifyjs/vuetify-loader',
    //     },
    //     {
    //       text: 'github',
    //       href: 'https://github.com/vuetifyjs/vuetify',
    //     },
    //     {
    //       text: 'awesome-vuetify',
    //       href: 'https://github.com/vuetifyjs/awesome-vuetify',
    //     },
    //   ],
    //   importantLinks: [
    //     {
    //       text: 'Documentation',
    //       href: 'https://vuetifyjs.com',
    //     },
    //     {
    //       text: 'Chat',
    //       href: 'https://community.vuetifyjs.com',
    //     },
    //     {
    //       text: 'Made with Vuetify',
    //       href: 'https://madewithvuejs.com/vuetify',
    //     },
    //     {
    //       text: 'Twitter',
    //       href: 'https://twitter.com/vuetifyjs',
    //     },
    //     {
    //       text: 'Articles',
    //       href: 'https://medium.com/vuetify',
    //     },
    //   ],
    //   whatsNext: [
    //     {
    //       text: 'Explore components',
    //       href: 'https://vuetifyjs.com/components/api-explorer',
    //     },
    //     {
    //       text: 'Select a layout',
    //       href: 'https://vuetifyjs.com/getting-started/pre-made-layouts',
    //     },
    //     {
    //       text: 'Frequently Asked Questions',
    //       href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
    //     },
    //   ],
    // }),
  

   
</script>
