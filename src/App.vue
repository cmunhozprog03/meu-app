<template>
  <div id="app">
    <h1>Bem-vindo ao meu primeiro projeto!</h1>
    <button @click="entrar">Entrar</button>
    
    <Usuario :nome="nome"/>

    

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
      nome: 'Chris teste'
    }
  },
  methods:{
    entrar(){
      this.nome = 'Curso VueJS';
    }
  }
 
}
</script>

<style scoped>
  
</style>