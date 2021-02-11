<template>
  <div id="usuario">

    <h2>Olá PROP: {{nome.split('')}}!</h2>

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
  }
}
</script>

<style scoped>
  h2{
    color: red;
    }
</style>