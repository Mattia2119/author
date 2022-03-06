<template>
    <section>
        <div class="top-container">
           <h2>Upcoming Events</h2>
           <p>meet the author in person</p>
        </div>

        <div class="bottom-container">
            <div class="card">
              <img src="../../assets/style/img/event-05-400x240.jpg" alt="">
              <h4>Chicago Book Signing</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing 
                elit. Veniam accusantium natus facilis odit
                numquam fugiat architecto.</p>
            </div>

            <div class="card">
              <img src="../../assets/style/img/event-04-400x240.jpg" alt="">
              <h4>Meet & Greet With Amanda</h4>
               <p>Lorem ipsum dolor sit amet consectetur adipisicing 
                elit. Veniam accusantium natus facilis odit
                numquam fugiat architecto.</p>
            </div>

            <div class="card">
              <img src="../../assets/style/img/event-07-400x240.jpg" alt="">
              <h4>Open Book Dialogues</h4>
               <p>Lorem ipsum dolor sit amet consectetur adipisicing 
                elit. Veniam accusantium natus facilis odit
                numquam fugiat architecto.</p>
            </div>
        </div>

    </section>
</template>

<script>
export default {
 name: "FourthJumbo"
}
</script>

<style lang="scss" scoped>

@import "../../assets/style/variables.scss";

section {
    height: 600px;
    background-color: $DawnPink;
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
            color: $saffron;
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
             background-color: white;
             margin: 0 20px;
              img {
                  width: 100%;
              }
            h4 {
                text-align: center;
                margin: 15px 0px;
            }
            p {
                text-align: center;
            }
         }
    }
}

</style>