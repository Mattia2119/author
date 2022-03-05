<template>

  <main> 
    <FirstJumbo/>
    <SecondJumbo/>
    <ThirdJumbo/>
    <FifthJumbo/>
  </main>


</template>

<script>
 import FirstJumbo from "./partials/FirstJumbo.vue"
 import SecondJumbo from "./partials/SecondJumbo.vue"
 import ThirdJumbo from "./partials/ThirdJumbo.vue"
 import FifthJumbo from "./partials/FifthJumbo.vue"
 

  export default {
  name: "MyMain",
  components: {
    FirstJumbo,
    SecondJumbo,
    ThirdJumbo,
    FifthJumbo
  }
  }
</script>

<style lang="scss" scoped> 


</style>