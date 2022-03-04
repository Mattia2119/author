<template>
<section class="first-jumbo">
 <div class="text-container">
      <h1>More About Damon Vaughn</h1>
      <p>Damon Vaughn is a professor at the University of Toronto
        a clinical psychologist and the author of the multi-million 
        copy bestseller "The story of my life"
      </p>
      <button>Meet the author</button>
      <SponsorsLine/>
    </div>
</section>
    
</template>

<script>

import SponsorsLine from "./sub-partials/SponsorsLine.vue"

export default {
 name: "FirstJmbo",
 components: {
      SponsorsLine,
    }
}
</script>

<style lang="scss" scoped>
 
 @import "../../assets/style/variables.scss";

 .first-jumbo {
   height: 500px;
   display: flex;
   justify-content: center;
   align-items: center;
   flex-direction: column;
   position: relative;
    .text-container {
      display: flex;
      align-items: center;
      flex-direction: column;
      width: 60%;
        h1 {
          font-family: 'Comforter Brush';
                color: $saffron;
                font-size: 50px;
        }
        p {
          font-family: 'Segoe UI','Open Sans', 'Helvetica Neue', sans-serif;
          text-align: center;
          margin: 10px 0px;
        }
        button {
          border: none;
          border-radius: 4px;
          background-color: $keppel;
          color: #ffff;
          height: 40px;
          width: 180px;
          margin-top: 40px;
           &:hover {
              filter: drop-shadow(0 0 0.70rem $keppel);
           }
        }
    }
 }

</style>