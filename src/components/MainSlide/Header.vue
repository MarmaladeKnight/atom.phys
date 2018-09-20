<template>
  <div class="header">
    <img id="logo" alt="Vue logo" src="../../assets/logo.png">
    <div>
        <h1>
            Atom.Phys
        </h1>
        <p>
            Конструктор атомов для уроков физики и химии
        </p>
    </div>
    
    
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
    .header {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;   
    }

    h1, p {
        margin: 0px;
        padding: 0px;
        color: #5D5D5D;
        font-weight: bold;
    }
    #logo {
        display: inline;
        width: 100px;
        height: 100px;
        margin-right: 15px; 
    }
</style>
