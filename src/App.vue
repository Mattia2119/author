<template>
  <div id="app">
    <MyHeader :links="links"/>
    <MyMain/>
  </div>
</template>

<script>

import MyHeader from "./components/MyHeader.vue"
import MyMain from "./components/MyMain.vue"

export default {
  name: 'App',
  data() {
   return {
        links: [
          {
             text: "Home",
             url: "#",
          },
          {
             text: "About Me",
             url: "#",
          },
          {
             text: "Testimonials",
             url: "#",
          },
          {
             text: "My Blog",
             url: "#",
          },
          {
             text: "Meetups",
             url: "#",
          },
          {
             text: "Shop",
             url: "#",
          },
          {
             text: "Contact Me",
             url: "#",
          },
        ]
   }
  },
  components: {
    MyHeader,
    MyMain
  }
}
</script>

<style lang="scss">

 @import "./assets/style/generals.scss";
 @import url('https://fonts.googleapis.com/css2?family=Comforter+Brush&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;1,400&display=swap');
 @import url('https://fonts.googleapis.com/css2?family=Comforter+Brush&family=Playfair+Display:wght@700&family=Roboto+Slab:wght@800&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;1,400&display=swap');

</style>
 