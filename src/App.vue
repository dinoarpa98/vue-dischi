<template>
 <body>
  <div>
    <header>
      <HeaderComp/>
    </header>

    <main>
      <div class="cards">
       <GrigliaDischi/>
      </div>
    </main>

  </div>
</body>

</template>

<script>
  import HeaderComp from './components/HeaderComp.vue'
  import GrigliaDischi from './components/GrigliaDischi.vue'
  import "bootstrap"

  export default {
    name: 'App',
    components: {
      HeaderComp,
      GrigliaDischi
    }
  }
</script>


<style lang="scss">
  @import "bootstrap/dist/css/bootstrap.min.css";
  
  body{
    background-color: #202D3B;
  }
</style>