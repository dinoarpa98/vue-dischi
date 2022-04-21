<template>
<div class="container">
  <div class="row row-cols-5 text-white">
     
      <div class="bg-blue px-2 m-4" v-for="(element, index) in dischi" :key="index">
          <img :src="element.poster" class="img-fluid" alt="">
          <h4>{{element.title}}</h4>
          <p class="text-muted">{{element.author}}</p>
          <p class="text-muted">{{element.year}}</p>
      </div>
      
  </div>
</div>
</template>

<script>

import axios from 'axios'

export default {
  
  name: 'GrigliaDischi',
  data(){
      return{
          dischi:[]
      }
  },
  created(){
      axios.get( 'https://flynn.boolean.careers/exercises/api/array/music' )
      .then( ( res )=>{
          this.dischi = res.data.response
      })
  }

}
</script>

<style scoped lang="scss">
 .bg-blue{
     background-color:#2F3A46 ;
 }
</style>