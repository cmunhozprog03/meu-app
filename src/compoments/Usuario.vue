<template>
  <div id="usuario">

    <h2>Olá {{nome}}!</h2>

  </div>
</template>

<script>
export default {
  name: 'Usuario',
  props: ['nome']
}
</script>

<style scoped>
  h2{
    color: red;
    }
</style>