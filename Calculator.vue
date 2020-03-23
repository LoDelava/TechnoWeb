<template>
  <div id="cal">
    <input v-model="nombre1" type="value" placeholder="Entier 1">
    <input v-model="signe" placeholder="Signe">
    <input v-model="nombre2" type="value" placeholder="Entier 2">
    <span> {{nombre1}} {{signe}} {{nombre2}} = {{calcul}} </span>
    <br>
    <br>
    <input v-model="distance" type="value" placeholder="Distance">
    <select v-model="unite" id="unit-select">
      <option value="">--Choisir une unite de mesure--</option>
      <option value="km">km</option>
      <option value="m">m</option>
      <option value="cm">cm</option>
      <option value="mm">mm</option>
    
    </select>
    <br>
    <span> {{distance}} {{unite}} = {{convertit}} </span>
    <br>
  </div>
</template>

<script>


export default {
  name: 'App',
  data:function(){
    return{
      distance: 1,
      unite: "km",
      nombre1: 2,
      signe:"+",
      nombre2: 2
    }
  },
  computed:{
    convertit(){
      if(this.unite=="km"){
        return[this.distance*1000,this.distance*100000,this.distance*1000000]
      }
      if(this.unite=="m"){
        return[this.distance/1000,this.distance*100,this.distance*1000]
      }
      if(this.unite=="cm"){
        return[this.distance/100000,this.distance/100,this.distance*10]
      }
      if(this.unite=="mm"){
        return[this.distance/1000000,this.distance/1000,this.distance/10]
      }
      return 0;
    },
    calcul(){
      if(this.signe=="+"){
        return parseInt(this.nombre1) + parseInt(this.nombre2);

      }
      if(this.signe=="*"){
        return parseInt(this.nombre1) * parseInt(this.nombre2);

      }
      if(this.signe=="/"){
        return parseInt(this.nombre1) / parseInt(this.nombre2);

      }
      if(this.signe=="-"){
        return parseInt(this.nombre1) - parseInt(this.nombre2);

      }
      return 0;
    }
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
