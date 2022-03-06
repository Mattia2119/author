<template>

  <main> 
    <FirstJumbo/>
    <SecondJumbo/>
    <ThirdJumbo/>
    <FourthJumbo/>
    <FifthJumbo/>
    <SixthJumbo/>
    <SeventhJumbo/>
  </main>


</template>

<script>
 import FirstJumbo from "./partials/FirstJumbo.vue"
 import SecondJumbo from "./partials/SecondJumbo.vue"
 import ThirdJumbo from "./partials/ThirdJumbo.vue"
 import FourthJumbo from "./partials/FourthJumbo.vue"
 import FifthJumbo from "./partials/FifthJumbo.vue"
 import SixthJumbo from "./partials/SixthJumbo.vue"
 import SeventhJumbo from "./partials/SeventhJumbo.vue"
 

  export default {
  name: "MyMain",
  components: {
    FirstJumbo,
    SecondJumbo,
    ThirdJumbo,
    FourthJumbo,
    FifthJumbo,
    SixthJumbo,
    SeventhJumbo
  }
  }
</script>

<style lang="scss" scoped> 


</style>