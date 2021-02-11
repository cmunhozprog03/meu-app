<template>
  <div id="app">
    <h1>Bem-vindo ao meu primeiro projeto!</h1>
    <p>Componente App: {{nome}}</p>
    <button @click="entrar">Entrar</button>
    
    <Usuario :nome="nome" @nomeCurso="nome = $event" />

    

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
      nome: 'Chris'
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