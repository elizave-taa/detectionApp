<template>
    <global-header/>
    <div class="main-container">
      <div id="main-image" class="slideInLeft">
        <img class="image" src="../assets/main-image.png" alt="main-image">
        <div class="app-name">RECYCLE DETECTION</div>
        <div class="slogan">take care<br>of nature</div>
      </div>
      <img @click="scrollDown" class="arrow" src="../assets/scrollDown.svg" alt="down">
    </div>
  <div class="main-container">

  </div>
</template>

<script>
import GlobalHeader from './GlobalHeader.vue'
export default {
  name: 'HelloWorld',
  components: {
    GlobalHeader
  },
  methods: {
    scrollDown() {
      window.scrollTo({
        top: window.innerHeight,
        behavior: 'smooth'
      });
    }
  }
}
</script>

<style scoped>
.main-container {
  background-color: #738f56;
  top: 0;
  left: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
.image {
  width: 75vw;
  height: 450px;
}
.slideInLeft {
  animation: slideInLeftAnimation 1s forwards;
}
@keyframes slideInLeftAnimation {
  from {
    transform: translateX(-100%);
  }
  to {
    transform: translateX(0);
  }
}
div#main-image {
  position: relative;
  margin-top: 50px;
}
.app-name {
  position: absolute;
  top: 10px;
  color: #FF7800;
  font-size: 68px;
  line-height: 80px;
  font-weight: bold;
  text-shadow: 0 1px 3px rgb(17, 65, 36);
}
.slogan {
  position: absolute;
  bottom: 15px;
  right: 15px;
  color: #ec9959;
  font-size: 48px;
  text-align: right;
  font-weight: 500;
  line-height: 40px;
}
.arrow {
  margin-top: 20px;
  width: 50px;
  height: 50px;
  cursor: pointer;
}
.arrow:hover {
  transform: scale(1.3);
}
</style>

