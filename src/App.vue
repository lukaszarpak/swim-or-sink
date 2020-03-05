<template>
  <div id="app">
    <Skills />
    <Reviews />
  </div>
</template>

<script>
import Skills from "./components/SkillsSection/Skills.vue";
import Reviews from "./components/CustomerReviews/Reviews.vue";

export default {
  name: "App",
  components: {
    Skills,
    Reviews
  }
};
</script>

<style lang="scss">
</style>
