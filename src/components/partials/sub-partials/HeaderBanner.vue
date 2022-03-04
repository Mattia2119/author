<template>
    <div class="container">
         <div class="image-box">
             <img src="../../../assets/style/img/book-widget.png">
         </div>
         <div class="text-box">
             <h1>Latest Book Release</h1>
             <p class="reference">D. VAUGHN AUTOBIOGRAPHY</p>
             <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vitae quod, aliquid recusandae numquam.</p>
         </div>
         <div class="btns-container">
            <button class="left"><i class="fa-brands fa-amazon"></i>Buy on Amazon</button>
            <button class="right"><i class="fa-brands fa-apple"></i>Buy on AppStore</button>
         </div>
    </div>
</template>

<script>
export default {
 name: "HeaderBanner"
}
</script>

<style lang="scss" scoped>

@import "../../../assets/style/variables.scss";

 .container {
     background-color: white;
     height: 320px;
     width: 550px;
     position: absolute;
     right: 0;
     bottom: 0;
     display: flex;
     flex-wrap: wrap;
     justify-content: center;
      .image-box {
          width: calc(100% / 2);
          float: left;
          display: flex;
          justify-content: flex-end;
          align-items: center;
           img {
               height: 80%;
           } 
      }
      .text-box {
          width: calc(100% / 2);
          float: right;    
          justify-content: flex-start;
          align-items: center;   
            h1 {
                font-size: 24px;
                font-family: 'Playfair Display', serif ;
                color: black;
                margin-top: 14%;
            }
            .reference {
                font-size: 14px;
                color: $saffron;
                margin: 3% 0px;
            }
            p {
                margin-top: 8%;
                font-family:'Segoe UI','Open Sans', 'Helvetica Neue', sans-serif;
                font-size: 18px;
            }
      }
      button {
          height: 40px;
          width: 200px;
          font-size: 14px;
          border: none;
          margin-bottom: 30px;
          border: 1px solid $keppel;
             &:hover {
                 filter: drop-shadow(0 0 0.15rem $keppel);
             }
           i {
               margin-right: 10px;
           }
      }
      .left {
                border-top-left-radius: 6px;
                border-bottom-left-radius: 6px;
                margin-right: 1px;
           }
           .right {
                border-top-right-radius: 6px;
                border-bottom-right-radius: 6px;
                margin-left: 1px;
           }
 }

</style>