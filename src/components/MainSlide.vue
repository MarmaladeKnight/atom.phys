<template>
  <div class="main_slide">
    <Header/>
    <Downloads/>
  </div>
</template>

<script>
import Header from './MainSlide/Header.vue'
import Downloads from './MainSlide/Downloads.vue'

export default {
  name: 'MainSlide',
  components: {
    Header,
    Downloads
  }
}
</script>

<style lang="scss">
    .main_slide {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 100vh;
        /*
        @media screen and (max-width: 426px){
            justify-content: space-evenly;
        }
        */
    }
</style>
