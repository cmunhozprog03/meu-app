<template>
  <div id="app">
    <h1>Bem-vindo ao meu primeiro projeto!</h1>
    
    <Usuario/>

    <h2>Olá eu sou um programador</h2>

  </div>
</template>

<script>
import Usuario from './compoments/Usuario';

export default {
  name: 'App',
  components:{
    Usuario
    
  },
  data(){
    return {
      name: 'Sujeito Programador'
    }
  },
 
}
</script>

<style scoped>
  h1{
    color: brown;
  }
</style>