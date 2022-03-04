<template>
 <nav>
     <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.url">{{link.text}}</a>
        </li>
        <!--<li><a href="#">{{}}</a></li>
        <li><a href="#">Testimonials</a></li>
        <li><a href="#">My Blog</a></li>
        <li><a href="#">Meetups</a></li>
        <li><a href="#">Shop</a></li>
        <li><a href="#">Contact Me</a></li>-->
        <li><a id="cart" href="#"><i class="fa-solid fa-cart-shopping"></i></a></li>
     </ul>
 </nav>

</template>

<script>
    export default {
    name: "MyNav",
    props: {'links': Object},
    }
</script>

<style lang="scss" scoped>
 @import "../../assets/style/variables.scss"; 
 nav {
     position: absolute;
     right: 70px;
     top: 20px;
 }

 ul {
      list-style: none;
      li{
        display: inline-block;
        font-family: 'Playfair Display', serif;
        font-size: 14px;
        font-weight: 600;
        margin-left: 20px;
        margin-right: 20px;
      }
        a {
          text-decoration: none;
          color: #ffff;
          padding-top: 20px;
          padding-bottom: 29px;
            &:hover{
              color: $saffron;
              border-top: 4px solid $saffron;
            }
        }
        #cart:hover{
          border-top: 4px solid white;
          color: white;
        }
    }
</style>