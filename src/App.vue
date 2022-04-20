<template>

  <div>
    <header>
      <HeaderComp />
    </header>

    <main>
      <div class="container">
      
      </div>
    </main>

  </div>


</template>

<script>
  import HeaderComp from './components/HeaderComp.vue'
  import "bootstrap"
  import axios from 'axios'

  export default {
    name: 'App',
    components: {
      HeaderComp
    }
  }
</script>


<style lang="scss">
  @import "bootstrap/dist/css/bootstrap.min.css";
  

  .container{
    background-color: #1E2D3B;
  }
</style>