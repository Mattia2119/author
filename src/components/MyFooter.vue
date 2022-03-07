<template>
  <footer>
      <MyLogo/>
      <div class="big-container">
            <div class="top-container">
                    <div class="text-container">
                        <div class="title">
                            <h4>About Me</h4>
                        </div>
                        <p>Lorem ipsum dolor sit amet consectetur 
                        adipisicing elit. Illo libero suscipit inventore 
                        voluptates vel impedit commodi, ea sequi,
                        nulla laudantium omnis quos facilis porro 
                        necessitatibus harum iure qui alias repellat?</p>
                    </div>

                    <div class="text-container center">
                        <div class="title centered">
                            <h4>Useful Links</h4>
                        </div>
                        <ul>
                            <li v-for="(link, index) in footerLinks" :key="index">
                             <a :href="link.url"><i class="fa-solid fa-angle-right"></i>&nbsp; {{link.text}}</a>
                            </li>
                            <!--<li><i class="fa-solid fa-angle-right"></i>&nbsp; Latest Books</li>
                            <li><i class="fa-solid fa-angle-right"></i>&nbsp; Upcoming Events</li>
                            <li><i class="fa-solid fa-angle-right"></i>&nbsp; Recents Articles</li>
                            <li><i class="fa-solid fa-angle-right"></i>&nbsp; Business Enquiries</li>
                            <li><i class="fa-solid fa-angle-right"></i>&nbsp; Visit My Foundation</li>-->
                        </ul>          
                    </div>

                    <div class="text-container">
                        <div class="title">
                            <h4>Contact Info</h4>
                        </div>
                        <p>63E.Studebaker Street Boolingbrook, IL 60440</p>
                        <p>Phone:(800)000-0000</p>
                        <p>Mobile:(800)000-0000</p>
                        <p>Email:<b>info@your-company.com</b></p>
                        <p>
                            <i class="fa-brands fa-facebook-f"></i>
                            <i class="fa-brands fa-twitter"></i>
                            <i class="fa-brands fa-instagram"></i>
                            <i class="fa-brands fa-linkedin-in"></i>
                            <i class="fa-brands fa-youtube"></i>
                        </p>   
                    </div>
            </div>

            <div class="bottom-container">
              <p>&copy; Copyright 2012-2020 | Avada Theme by <b>ThemeFusion</b> | All Rights Reserved | Powered by <b>WordPress</b></p>
            </div>
        </div>

  </footer>
</template>

<script>

import MyLogo from "./partials/sub-partials/MyLogo.vue"

export default {
 name: "MyFooter",
 props: { 
     'footerLinks': Array
 },
 components: {
     MyLogo,
 }
}
</script>

<style lang="scss" scoped>

@import "../assets/style/variables.scss";

footer {
    height: 60vh;
    background-image: linear-gradient( to top, black, transparent), url("../assets/style/img/hero-07-2x.jpg");   
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    .big-container{
        height: 100%;
        width: 65%;
            .title{
                height: 50%;
                width: 100%;
                display: flex;
                align-items: end;
                h4 {
                    color: white;
                    text-transform: uppercase;
                    margin-bottom: 20px;
                }
            }
        p {
            color: white;
            font-size: 16px;
            margin-top: 10px;
            i{
                margin-right: 25px;
                margin-top: 10px;
            }
        }
        li {
            list-style: none;
            font-size: 16px;
            margin-bottom: 10px;
            
        }
        a {
            color: white;
            text-decoration: none;
             &:hover {
                 color: antiquewhite;
             }
        }
        .center {
            align-items: center;
        }
        .centered {
            justify-items: center;
            width: auto;
        }
        .top-container{
            height: 70%;
            width: 100%;
            display: flex;
            .text-container {
                height: 100%;
                width: calc(100% / 3);
                display: flex;
                flex-direction: column;
            }
        }
        .bottom-container{
            height: 30%;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
    }
}

</style>