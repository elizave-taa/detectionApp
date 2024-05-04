<template>
<div class="container">
  <div class="header">
    <div>
        <img class="logo" src="../assets/logo.svg">
    </div>
    <div class="links">
        <p>О нас</p>
        <p>Виды маркировок и значение</p>
        <p>Контакты</p>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'GlobalHeader',
  components: {
  },
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
    background-color: rgba(104, 131, 77, 0.55); 
    backdrop-filter: blur(40px);
    -webkit-backdrop-filter: blur(40px); 
    padding: 200px 10px;
}
.header{
}
</style>