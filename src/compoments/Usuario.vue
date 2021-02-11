<template>
  <div id="usuario">

    <h2>Olá PROP: {{nome}}!</h2>
    <button @click="curso">Nome Curso</button>

  </div>
</template>

<script>
export default {
  name: 'Usuario',
  props: {
    nome: {
      type: String,
      required: true
    }
  },
  methods:{
    curso(){
      this.nome = "Aprendendo Alemão";
      this.$emit('nomeCurso', this.nome);
    }
  }
}
</script>

<style scoped>
  h2{
    color: red;
    }
</style>