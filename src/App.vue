<template>
    <main>
        <!-- <MainTitle></MainTitle> -->
        <Downloads></Downloads>
    </main>
</template>

<script>
import MainSlide from './components/MainSlide.vue'
import MainTitle from './components/MainTitle.vue'
import Downloads from './components/Downloads.vue'


export default {
    name: 'app',
    components: {
        MainSlide,
        MainTitle,
        Downloads
    }
}
</script>

<style lang="scss">
    html, body {
        padding: 0px;
        margin: 0px;
        overflow-y: hidden;
    }

    main {
        display: flex;
        flex-direction: row;


        width: 200vw;
        height: 100%;
        overflow-y: hidden;
    }
</style>
