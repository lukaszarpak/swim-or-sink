<template>
  <div class="wrap">
    <h2>Nasze specjalności</h2>
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren.</p>
    <div class="container mx-auto">
      <div class="row">
        <Skill />
        <Skill />
        <Skill />
      </div>
    </div>
  </div>
</template>

<script>
import Skill from "./Skill.vue";
export default {
  name: "Skills",
  components: {
    Skill
  }
};
</script>

<style scoped lang="scss">
.wrap {
  background: linear-gradient(
    200deg,
    rgba(16, 44, 79, 1) 0%,
    rgba(33, 75, 124, 1) 100%
  );
  text-align: center;
  color: #fff;
  padding: 100px 0;
  > h2 {
    margin-bottom: 30px;
  }
  > p {
    width: 80%;
    max-width: 600px;
    margin: 0 auto 50px;
  }
}
</style>
