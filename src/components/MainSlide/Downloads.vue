<template>
  <div class="downloads">
    <h4>Доступно в </h4>
    <div class="download_items">
      <DownloadItem
        v-for="item in items"
        v-bind:key="item.index"
        v-bind:pic_name="item.path"
        v-bind:url="item.url">
      </DownloadItem>
    </div>
  </div>
</template>

<script>
import DownloadItem from './Downloads/DownloadItem.vue'

export default {
  name: 'Downloads',
  data: function () {
    return {
      items: [
        { path: 'WinStore.png', url: 'https://www.microsoft.com/ru-ru/p/atomphys/9p9dv88hb9s8' },
        { path: 'GooglePlay.png', url: 'https://play.google.com/store/apps/details?id=com.CowboyBebop.AtomPhys' },
        { path: 'AppStore.png', url: 'https://itunes.apple.com/ru/app/atom-phys-%D0%BA%D0%BE%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D0%BE%D1%80-%D0%B0%D1%82%D0%BE%D0%BC%D0%BE%D0%B2/id1355454097' },
        { path: 'Mash.png', url: 'https://uchebnik.mos.ru/material_view/game_apps/8316' }
      ]
    }
  },
  components: {
    DownloadItem
  }
}
</script>

<style lang="scss" scoped>
.downloads {
  height: 200px;
  text-align: center;
}
.download_items {
  width: 500px;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  @media screen and (max-width: 426px){
    width: 250px;
  }
}
</style>
