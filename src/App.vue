<template>
    <MainSlide/>
</template>

<script>
import MainSlide from './components/MainSlide.vue'

export default {
  name: 'app',
  components: {
    MainSlide
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=PT+Sans:400,700&subset=cyrillic');

html, body {
  padding: 0px;
  margin: 0px;
  width: 100%;
  max-height: 100%;
  font-family: 'PT Sans', sans-serif;
  background-color: rgb(245, 245, 245);
  box-shadow: inset 0px 4px 100px rgba(0, 0, 0, 0.25);
  color: #5D5D5D;
}
</style>
