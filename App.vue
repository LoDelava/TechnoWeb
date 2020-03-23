<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Formula/>
    <!--<Filtre/>-->
    <!--<MetersForm/>-->
  </div>
</template>

<script>
import Formula from './components/Formula.vue'
//import Filtre from './components/Filtre.vue'
/*import MetersForm from './components/MetersForm.vue' */

export default {
  name: 'App',
  components: {
    Formula,
    //Filtre,
    //MetersForm
    
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
