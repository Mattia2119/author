<template>
  <section>
    <div class="container-big">

          <div class="top-container">
                <div class="text-box">
                <h2>Recent Articles</h2>
                <p>Read the last entries</p>
                </div>
                <button>All Articles</button>
            </div>
          <div class="bottom-container">
               <div class="left-card">
                   <img src="../../assets/style/img/20-Tips-800x471.jpg" alt="">

                   <div class="text-box">
                        <h3>20 Creativity Tips</h3>
                        <p class="date">By Admin | October 24th,2019 | Categories: <b>Event, Tips & Tricks</b></p>
                        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. 
                            Explicabo quis tenetur deleniti necessitatibus ut laboriosam, praesentium.</p>
                    </div>

               </div>
               <div class="right-card">

                <img src="../../assets/style/img/thumb-13-2x-320x202.jpg" alt="">
                <div class="text-box">
                <h3>What's On Your Booklist?</h3>
                <p class="date">October 24th,2019 | 0 Comments</p>
                </div>

                <img src="../../assets/style/img/thumb-08-2x-320x202.jpg" alt="">
                <div class="text-box">
                <h3>Istanbul Travel Guide</h3>
                <p class="date">October 24th,2019 | 0 Comments</p>
                </div>
               </div>
          </div>
                
    </div>
  </section>
</template>

<script>
export default {
 name: "SeventhJumbo"
}
</script>

<style lang="scss" scoped>

@import "../../assets/style/variables.scss";

section {
    height: 900px;
    background-color: $DawnPink;
     .container-big{
         width: 80%;
         margin: auto;
         height: 100%;
         .top-container{
             height: 20%;
             width: 100%;
             display: flex;
             align-items: flex-end;
             justify-content: space-between;
              button{
                   background-color: $saffron;
                   color: #ffff;
                   height: 40px;
                   width: 200px;
                   font-size: 14px;
                   border: none;
                   border-radius: 4px;
                   margin-bottom: 35px;
                    &:hover {
                        filter: drop-shadow(0 0 0.70rem $saffron)
                    }              
              }
              p {
                text-transform: uppercase;
                color: $keppel;
                margin-top: 10px;
                font-size: 16px;
                margin-bottom: 30px;
              }

         }
        .bottom-container{
            height: 70%;
            width: 100%;
             .left-card{
                 background-color: white;
                 height: 100%;
                 width: 65%;
                 float: left;
                 display: flex;
                 flex-direction: column;
                 align-items: center;
                 justify-content: center;
                  img{
                      height: 70%;
                      width: 90%;
                      margin: 10px auto;
                  }
                  .text-box{
                      width: 90%;
                  }
                  p {
                      font-size: 14px;
                      margin: 10px auto;
                  }

             }
             .right-card{
                 background-color: white;
                 height: 100%;
                 width: 31%;
                 float: right;
                 display: flex;
                 flex-direction: column;
                 align-items: center;
                 justify-content: center;   
                 img {
                     height: 35%;
                     width: 85%;
                     margin: 10px auto;
                 }
                 .text-box {
                     width: 80%;
                 }
                 p {
                     font-size: 14px;
                     margin: 10px auto;
                 }
             }
        }
     }
}

</style>