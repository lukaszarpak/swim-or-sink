<template>
  <div class="wrap">
    <h2>Opinie klientów</h2>
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren.</p>
    <div class="container mx-auto">
      <div class="row">
        <Review />
        <Review />
        <Review />
        <Review />
        <Review />
        <Review />
      </div>
    </div>
  </div>
</template>

<script>
import Review from "./Review.vue";
export default {
  components: {
    Review
  }
};
</script>

<style lang="scss" scoped>
.wrap {
  padding: 100px 0;
  text-align: center;
  > h2 {
    margin: 50px 0;
  }
  > p {
    width: 80%;
    max-width: 600px;
    margin: 0 auto 50px;
  }
}
</style>