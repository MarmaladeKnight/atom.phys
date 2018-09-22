<template>
  <div class="slide1">
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
    .slide1 {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100vw;
        height: 100vh;
    }
</style>
