<template>
   <section>
     <div class="container">
         <div class="card-left">
             <img src="../../assets/style/img/audible-app-2x.png" alt="">
         </div>
         <div class="card-right">
           <h1>New Audiobook</h1>
           <p class="orange-text">No time to read? No problem listen to it</p>
           <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Officia 
               provident quas non atque sint Lorem ipsum, dolor sit amet consectetur 
               adipisicing elit. Labore dignissimos et nulla similique iusto, temporibus
                nihil porro nisi sit accusantium nemo? Ipsam
                nisi vitae quaerat nulla quae doloremque, explicabo iste.</p> 
                <div class="img-container">
                    <div class="img-box">
                      <img src="../../assets/style/img/audible-logo.png" alt="">
                    </div>
                    <div class="img-box">
                       <img src="../../assets/style/img/bn-logo-tall.png" alt="">
                    </div>
                    <div class="img-box">
                        <img src="../../assets/style/img/kindle-logo-tall.png" alt="">
                    </div>
                </div>
         </div>
     </div>
   </section>
</template>

<script>
export default {
 name: "SecondJumbo"
}
</script>

<style lang="scss" scoped>

 @import "../../assets/style/variables.scss";

 section {
     height: 400px;
     background-image:linear-gradient( to top, black, transparent), url("../../assets/style/img/banner.jpg");
     background-size: cover;
     background-repeat: no-repeat;
      .container {
          width: 50%;
          height: 100%;
          margin: auto;
          display: flex;
          align-items: center;
           .card-left{
               width: calc(100% / 2);
               height: 100%;
               float: left;
               position: relative;
               display: flex;
               flex-direction: column;
               align-items: center;
               justify-content: center;
                img {
                    height: 90%;
                    position: absolute;
                    bottom: 0px;
                    left: 21px;
                }
           }
           .card-right{
               width: calc(100% / 2);
               height: 50%;
               float: right;
               position: relative;
               display: flex;
               flex-direction: column;
               align-items: center;
               justify-content: center;
                h1 {
                    font-size: 30px;
                    color: white;
                }
                .orange-text{
                  color: $saffron;
                  text-transform: uppercase;
                  margin: 15px 0px;
                  font-size: 12px;
                  font-weight: 600;
                }
                p {
                    color: grey;
                    font-size: 12px;
                    text-align: center;
                }
                .img-container{
                   width: 100%;
                   height: 100px;
                     .img-box{
                       width: calc(100% / 3);
                       height: 100%;
                       float: left;
                       display: flex;
                       justify-content: center;
                       align-items: center;
                          img {
                              height: 60%;
                          }
                     }
                }
           }

      }
 }

</style>