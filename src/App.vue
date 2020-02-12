<template>
  <div id="app"  class="container mx-auto">
    <h1>Meu primeiro Math App.vue</h1>
   <!-- <div> header</div>
    <HelloWorld msg="Vue.js aula da thais" :n="4"/>-->
    <div class="cards"> 
      <Quadrado :numero="5"/>
      <Cubo :numero="5"/>
    </div>
    
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Quadrado from './components/Quadrado.vue'
import Cubo from './components/Cubo.vue'

export default {
  name: 'app',
  components: {
    //HelloWorld,
    Quadrado,
    Cubo
  },data(){
    return { n : 7}
  }
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px;
}

.cards{
  padding: 24px;
  display: flex;
  justify-content:space-between; 
  margin: auto;
}
</style>
