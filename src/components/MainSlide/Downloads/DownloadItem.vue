<template>
  <div class="item_wrapper">
    <a :href="url" class="ball_wrapper">
      <img
      class="download_item"
      :alt="imagePath"
      :src="imagePath">
    </a>
    <div class="item_shadow"></div>
  </div>
</template>

<script>

export default {
  name: 'DownloadItem',
  props: ['pic_name', 'url'],
  computed: {
    imagePath: function () {
      return 'static/' + this.pic_name
    }
  }
}

</script>

<style lang="scss" scoped>
    .item_wrapper {
        background-color: red;
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .ball_wrapper{
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .ball_wrapper:hover + .item_shadow{
        width: 80px;
    }

    .download_item {
        position: absolute;
        top: 0;
        z-index: 2;
        width: 100px;
        height: 100px;
        transition: 0.2s ease-in-out;
    }

    .download_item:hover {
        top: 4px;
    }

    .item_shadow {
        position: absolute;
        top: 95px;
        z-index: 1;
        width: 70px;
        height: 20px;
        border-radius: 100%;
        background-color: rgba(0, 0, 0, 0.5);
        transition: 0.2s ease-in-out;
    }
</style>
