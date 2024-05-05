<template>
<div class="container">
  <div class="row">
    <img class="logo" src="../assets/logo.svg">
    <div class="links">
        <p class="header-item" @onclick="aboutUs">О нас</p>
        <p class="header-item">Виды маркировок и значение</p>
        <p class="header-item">Контакты</p>
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
  },
  methods: {
    aboutUs() {
      window.scrollTo({
        top: window.innerHeight,
        behavior: 'smooth'
      });
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
    background-color: rgba(95, 122, 71, 0.59);
    backdrop-filter: blur(40px);
    -webkit-backdrop-filter: blur(40px);
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    justify-content: center;
    display: flex;
    z-index: 10;
}
.row {
  width: 75vw;
  justify-content: space-between;
  display: flex;
}
.logo {
  width: 120px;
  height: 60px;
}
.links {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 60%;
  color: #FEFAE0;
  font-size: 15px;
}
.header-item:hover {
  transform: scale(1.1);
  cursor: pointer;
}
</style>