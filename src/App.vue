<template>
    <MainSlide></MainSlide>
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
@import url('https://fonts.googleapis.com/css?family=PT+Sans');

html, body {
  padding: 0px;
  margin: 0px;
  font-family: 'PT Sans', sans-serif;
  background-color: rgb(245, 245, 245); 
  box-shadow: inset 0px 4px 100px rgba(0, 0, 0, 0.25);
}
</style>
