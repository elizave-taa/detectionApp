<template>
  <div class="hello">
    <GlobalHeader/>
    <ScrollButtonUp/>
  </div>
</template>

<script>
import ScrollButtonUp from './ScrollButtonUp.vue'
import GlobalHeader from './GlobalHeader.vue'
export default {
  name: 'HelloWorld',
  components: {
    ScrollButtonUp, GlobalHeader
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
