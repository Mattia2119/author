<template>
 <section>

        <div class="top-container">
           <h2>Dig A Little Deeper Into Damon Vaughn</h2>
           <p>find out more about the author himself</p>
        </div>

        <div class="bottom-container">
            <div class="card left">
              <div class="text-box">
                <h2>About Me</h2>
                <hr>
                <p>Vestibulum ante ipsum primis</p>
              </div>
            </div>

            <div class="card center">
              <div class="text-box">
                <h2>My Latest Book</h2>
                <hr>
                <p>Vestibulum ante ipsum primis</p>
              </div>
            </div>

            <div class="card right">
              <div class="text-box">
                <h2>Book Signing</h2>
                <hr>
                <p>Vestibulum ante ipsum primis</p>
              </div>
            </div>
        </div>


 </section>
</template>

<script>
export default {
name: "SixthJumbo"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";

section {
    height: 600px;
    .top-container{
        height: 22%;
        width: 80%;
        margin: auto;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
            h2{
            font-family: 'Playfair Display', serif ;
            color: black;
            margin-bottom: 10px;
            }
            p{
            color: $keppel;
            text-transform: uppercase;
            font-size: 16px;
            }
    }
    .bottom-container {
        height: 70%;
        width: 80%;
        margin: auto;
        display: flex;
        flex-wrap: wrap;
        align-items: center;
         .card{
             height: 90%;
             width: calc(90% / 3);
             margin: 0 20px;
             border-bottom-right-radius: 40px;
             display: flex;
             align-items: flex-end;
             justify-content: center;
              .text-box{
                  display: flex;
                  flex-direction: column;
                  align-items: center;
                  text-align: center;
                  h2{
                      color: white;
                  }
                  hr{
                      width: 40px;
                      margin: 10px 0px;
                      height: 0.1;
                  }
                  p{
                     color: $saffron; 
                     font-size: 18px;
                     margin-bottom: 30px;
                  }
              }
         }
         .left {
             background-image: linear-gradient(to top, black, transparent), url("../../assets/style/img/box-1.jpg");
             background-size: cover;
         }
         .center {
             background-image: linear-gradient(to top, black, transparent), url("../../assets/style/img/box-4.jpg");
             background-size: cover;
         }
         .right {
             background-image: linear-gradient(to top, black, transparent), url("../../assets/style/img/box-3.jpg");
             background-size: cover;
         }
    }
}

</style>