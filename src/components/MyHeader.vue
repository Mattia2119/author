<template>
  <header>
      <MyLogo/>  
      <MyNav :links='links'/>
      <HeaderBanner/>
      <div class="text-container">
          <h1>Damon Vaughn</h1>
          <h2>Best-selling author and the most influential public
              intellectual in the western world right now.
          </h2>
          <p>-The New York Times</p>
          <button id="button-left"><i class="fa-solid fa-arrow-left"></i></button>
          <button id="button-right"><i class="fa-solid fa-arrow-right"></i></button>
      </div>
  </header>
 
</template>

<script>

import MyLogo from "./partials/sub-partials/MyLogo.vue"
import MyNav from "./partials/MyNav.vue"
import HeaderBanner from "./partials/sub-partials/HeaderBanner.vue"

export default {
 name: "MyHeader",
 props: { 
     'links': Array
 },
 components: {
     MyLogo,
     MyNav,
     HeaderBanner,
 }
}


</script>

<style lang="scss" scoped>


 @import "../assets/style/variables.scss";

header {
    height: 100vh;
    background-image: linear-gradient( to top, black, transparent), url("../assets/style/img/hero-07-2x.jpg");   
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
       
    .text-container {
      
      width: 700px;
      margin-left: 8%;
      margin-top: 2%;

        h1 {
            font-family: 'Comforter Brush';
            color: $saffron;
            font-size: 70px;
        }
        h2 {
            color: #ffff;
            font-size: 40px;
            font-family: 'Playfair Display', serif;
            font-weight: 600;
        }
        p {
            color:$suva-grey;
            margin-top: 30px;
            font-family: 'Segoe UI','Open Sans', 'Helvetica Neue', sans-serif;
            font-weight: 400;
        }
        #button-left {
          border: none;
          background-color: black;
          color: white;
          border-top-left-radius: 5px;
          border-bottom-left-radius: 5px;
          height: 50px;
          width: 50px;
          cursor: pointer;
        }
        #button-right {
          border: none;
          background-color: black;
          color: white;
          border-top-right-radius: 5px;
          border-bottom-right-radius: 5px;
          margin: 30px 1px;
          height: 50px;
          width: 50px;
          cursor: pointer;
        }
    
    }
      
}

</style>