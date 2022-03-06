<template>

  <main> 
    <FirstJumbo/>
    <SecondJumbo/>
    <ThirdJumbo/>
    <FourthJumbo/>
    <FifthJumbo/>
  </main>


</template>

<script>
 import FirstJumbo from "./partials/FirstJumbo.vue"
 import SecondJumbo from "./partials/SecondJumbo.vue"
 import ThirdJumbo from "./partials/ThirdJumbo.vue"
 import FourthJumbo from "./partials/FourthJumbo.vue"
 import FifthJumbo from "./partials/FifthJumbo.vue"
 

  export default {
  name: "MyMain",
  components: {
    FirstJumbo,
    SecondJumbo,
    ThirdJumbo,
    FourthJumbo,
    FifthJumbo
  }
  }
</script>

<style lang="scss" scoped> 


</style>