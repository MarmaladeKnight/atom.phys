<template>
  <div class="slide1">
    <Header></Header>
    <Downloads>
        <DownloadItem v-for="item in items"></DownloadItem>
    </Downloads>
  </div>
</template>

<script>
import Header from './MainSlide/Header.vue'
import Downloads from './MainSlide/Downloads.vue'
import DownloadItem from "./MainSlide/Downloads/DownloadItem.vue"

export default {
  name: 'MainSlide',
  data: function() {
    return {
        items: [
            { name: "GooglePLay"},
            { name: "AppStore"},
            { name: "Wintore"}
    ] }
  },    
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
