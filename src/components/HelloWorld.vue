<template>
    <global-header/>
    <div class="main-container">


      <div id="main-image">
        <img class="image" src="../assets/main-image.png" alt="main-image">
          <div class="app-name">RECYCLE DETECTION</div>
          <div class="slogan">take care<br>of nature</div>
      </div>


    </div>
</template>

<script>
import GlobalHeader from './GlobalHeader.vue'
export default {
  name: 'HelloWorld',
  components: {
    GlobalHeader
  },
}
</script>

<style scoped>
.main-container {
  background-color: #738f56;
  top: 0;
  left: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
.image {
  margin-top: 30px;
  width: 75vw;
  height: 450px;
}

div#main-image {
  position: relative;
}
.app-name {
  position: absolute;
  top: 30px;
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
</style>

