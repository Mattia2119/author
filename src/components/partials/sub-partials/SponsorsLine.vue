<template>
    <section>
        <div class="container">
            <div class="box">      
              <img src="../../../assets/style/img/ebay-logotan-2x-200x66.png" alt="">
             </div>

             <div class="box">
              <img src="../../../assets/style/img/audible-logotan-2x-200x66.png" alt="">
             </div>

             <div class="box">
               <img src="../../../assets/style/img/bb-logotan-2x-200x66.png" alt="">
             </div>

             <div class="box">
              <img src="../../../assets/style/img/kindlefire-logotan-2x-200x66.png" alt="">
             </div>
        </div>
    </section>
</template>

<script>
    export default {
    name: "SponsorsLine"
    }
</script>

<style lang="scss" scoped>
 
 @import "../../../assets/style/variables.scss";
 
 section {
     background-color: $DawnPink;
     height: 90px;
     display: flex;
     width: 100%;
     position: absolute;
     bottom: 0px;
      .container {
          height: 100%;
          width: 60%;
          margin: auto;
           .box {
               height: 100%;
               width: calc(100% / 4);
               display: flex;
               align-items: center;
               justify-content: center;
               float: left;
                img {
                    height: 40px;
                    width: 120px;
                }
           }
      }
 }


</style>

