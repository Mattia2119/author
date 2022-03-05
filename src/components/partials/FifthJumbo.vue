<template>
    <section>
        <div class="container">
            <div class="top">
              <h1>Subscribe To My Newsletter</h1>
              <p>Be notified about book signing tour dates</p>
            </div>

            <div class="half">
                <input type="text" placeholder=" Insert your email...*">
                <button>Subscribe</button>
            </div>

            <div class="bottom">
                <p>Lorem ipsum dolor sit, amet consectetur adiemus abectat proibizio
                    cunefactio innerit sumae.
                </p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
 name: "FifthJumbo"
}
</script>

<style lang="scss" scoped>

@import "../../assets/style/variables.scss";

section {
    height: 400px;
     background-image:linear-gradient( to top, black, transparent), url("../../assets/style/img/banner-2.jpg");
     background-size: cover;
     background-repeat: no-repeat;
      .container {
          width: 30%;
          height: 100%;
          margin: auto;
           .top {
               height: 50%;
               display: flex;
               flex-direction: column;
               justify-content: end;
                h1 {
                    color: white;
                    text-align: center;
                    font-size: 38px;
                    margin-bottom: 10px;
                }
                p {
                    text-transform: uppercase;
                    color: $saffron;  
                    text-align: center;
                    font-size: 14px;
                    margin-bottom: 10px;
                }
           }
           .half {
               height: 20%;
               display: flex;
               justify-content: space-between;
               align-items: center;
                input {
                    width: 62%;
                    height:60%;
                    border-radius: 6px;
                    border: none;
                }
                button {
                    width: 35%;
                    height: 60%;
                    background-color: $keppel;
                    border-radius: 6px;
                    color:white;
                    border: none;
                     &:hover {
                        filter: drop-shadow(0 0 0.70rem $keppel); 
                     }
                }
           }
           .bottom {
               height: 30%;
                p {
                    color: grey;
                    text-align: center;
                    margin-top: 20px;
                }

           }
      }
}

</style>