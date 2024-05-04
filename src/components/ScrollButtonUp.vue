<template>
  <button @click="nextSlide">Next Slide</button>
</template>

<script>
export default {
  name: 'ScrollButtonUp',
  methods: {
    nextSlide() {
      window.scrollTo({
        top: window.innerHeight,
        behavior: 'smooth'
      });
    }
  }
}
</script>
