<template>
  <div class="header">
    <img id="logo" alt="Atom.Phys" src="../../assets/logo.png">
    <div>
        <h1>
            Atom.Phys
        </h1>
        <h3>
            {{ $t('title') }}
        </h3>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data () { return { locale: 'en' } },
  watch: {
    locale (val) {
      this.$i18n.locale = val
    }
  }
}
</script>

<style lang="scss" scoped>
    .header {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;

        h1, h3 {
            margin: 0px;
            padding: 0px;
            font-weight: bold;
            user-select: none;
        }

        h1 {
            margin-top: -25px;
            font-size: 90px;

            @media screen and (max-width: 426px){
                margin-top: -5px;
                font-size: 30px;
            }
        }

        h3 {
            margin-top: -10px;
            @media screen and (max-width: 426px){
                margin-top: 0px;
                font-size: 14px;
            }
        }
        @media screen and (max-width: 426px){
            margin-top: -200px;
        }
    }

    #logo {
        display: block;
        width: 130px;
        height: 130px;
        margin-right: 15px;
        @media screen and (max-width: 426px){
            width: 90px;
            height: 90px;
        }
    }

    @media screen and (max-width: 426px){
        .header div {
            width: 180px;
        }
    }
</style>
