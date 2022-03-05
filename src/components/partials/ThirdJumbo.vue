<template>
  <section>
      <!--Inizio container superiore-->
        <div class="top-container">
            <div class="to-center">
                <div class="text-container">
                    <h1>What The Critics Say</h1>
                    <p>Testimonials from around the World</p>
                </div>
                <button>Read All Testimonials</button>
            </div>
        </div>
      <!--Fine container superiore-->

      <!--Inizio container inferiore-->
      <div class="bottom-container">

      <!--Parte sinistra-->
        <div class="left-container">
            <div class="card">
                <div class="card-text-container">

                    <h2>Best Author Of His Generation</h2>

                    <p>This Book will change your perspective of life.</p>

                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                        Soluta eius, odio beatae corrupti nisi qui
                        magni adipisci ex laborum laboriosam maxime 
                        provident recusandae? Expedita aliquid delectus 
                        quam iure dolorem assumenda?</p>

                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                        Cum neque natus aliquid tenetur,
                        sint blanditiis ducimus molestias recusandae accusamus 
                        saepe laborum modi laboriosam ullam excepturi dolor quasi
                        quidem! Numquam, eius?</p>

                    <span>Justine Kilpatrick</span>

                    <span class="green">The New York Times</span>
                </div>
            </div>
        </div>
        <!--Fine Parte Sinistra-->

        <!--Parte Destra-->
        <div class="right-container">
            <div class="half">
                <h3>A True Masterpiece, Bravo!</h3>
                <p>Lorem, ipsum dolor sit amet consectetur 
                adipisicing elit. Non eos obcaecati 
                accusantium exercitationem
                , magni deserunt, sunt odio, ipsa sint
                beatae quidem. Ratione cum possimus 
                autem maiores ducimus! In, corporis odio!</p>
            </div>
            <div class="little-container">
              <p> Gerald Hendley,
                  <span class="green">The Globe And Mail.</span>
              </p> 
            </div>


            <div class="half">
             <h3>A Unique view on the world</h3>
                <p>Lorem, ipsum dolor sit amet consectetur 
                adipisicing elit. Non eos obcaecati 
                accusantium exercitationem
                , magni deserunt, sunt odio, ipsa sint
                beatae quidem. Ratione cum possimus 
                autem maiores ducimus! In, corporis odio!</p>
            </div>
            <div class="little-container">
              <p> Mary Maxei,
                  <span class="green">The Globe And Mail.</span>
             </p> 
            </div>
        </div>
        <!--Fine Parte Destra-->

      </div>
      <!--Fine container inferiore--> 

  </section>
</template>

<script>
export default {
 name: "ThirdJumbo"
}
</script>

<style lang="scss" scoped>

@import "../../assets/style/variables.scss";

section {
    height: 800px;
     .top-container{
         height: 120px;
         width: 100%;
          .to-center{
              width: 70%;
              margin: auto;
              height: 100%;
              display: flex;
              justify-content: space-between;
              align-items: center;
               button {
                   background-color: $saffron;
                   color: #ffff;
                   height: 40px;
                   width: 250px;
                   font-size: 14px;
                   border: none;
                   border-radius: 4px;
                   margin-top: 20px;
                    &:hover {
                        filter: drop-shadow(0 0 0.70rem $saffron)
                    }
               }
               .text-container{
                   height: 100%;
                   width: 30%;
                   display: flex;
                   flex-direction: column;
                   justify-content: center;
                    p {
                        text-transform: uppercase;
                        color: $suva-grey;
                        margin-top: 10px;
                        font-size: 16px;
                    }
               }
          }
     }


    .bottom-container{
        width: 70%;
        margin: auto;
        height: 100%;
        display: flex;
        padding-bottom: 200px;
        .left-container {
            width: 50%;
            height: 100%;
            float: left;
            display: flex;
            justify-content: right;
            .card{
                background-image: linear-gradient( to top, black, transparent), url("../../assets/style/img/testimonial2-2x.jpg");
                background-position-x: right;
                background-size: cover;
                background-repeat: no-repeat;
                height: 100%;
                border-bottom-right-radius: 40px;
                display: flex;
                align-content: center;
                .card-text-container {
                width: 80%;
                height: 80%;
                margin: auto;
                    h2{
                        color: white;
                        padding-bottom: 15px;
                        border-bottom: 1px solid white;
                        font-size: 36px;
                    }
                    p {
                        margin: 20px 0px;
                        color: white;
                    }
                    span {
                        color: white;
                        margin-right: 8px;
                    }
                    .green {
                        color: $keppel;
                        font-size: 16px;
                    }
                }
            }
        }


        .right-container {
            width: 50%;
            height: 100%;
            float: left;
            .half {
                height: 40%;
                width: 90%;
                margin-left: 10%;
                background-color: $DawnPink;
                display: flex;
                align-items: center;
                justify-content: center;
                flex-direction: column;
                h3 {
                    margin-bottom: 20px;
                }
                 p {
                     text-align: center;
                 }
            }
            .little-container{
                height: 10%;
                width: 90%;
                margin-left: 10%;
                display: flex;
                align-items: center;
                 .green {
                    color: $keppel;
                    font-size: 17px;
                 }
            }
        }
    }    
}

</style>
