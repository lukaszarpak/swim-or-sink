<template>
  <div class="wrap">
    <h2>Opinie klientów</h2>
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren.</p>
    <div class="container mx-auto">
      <div class="row">
        <Review
          :reviewimg="reviewimg1"
          :nameOnReview="nameOnReview1"
          :textOnReview="textOnReview1"
        />
        <Review
          :reviewimg="reviewimg2"
          :nameOnReview="nameOnReview2"
          :textOnReview="textOnReview2"
        />
        <Review
          :reviewimg="reviewimg3"
          :nameOnReview="nameOnReview3"
          :textOnReview="textOnReview3"
        />
        <Review
          :reviewimg="reviewimg4"
          :nameOnReview="nameOnReview4"
          :textOnReview="textOnReview4"
        />
        <Review
          :reviewimg="reviewimg5"
          :nameOnReview="nameOnReview5"
          :textOnReview="textOnReview5"
        />
        <Review
          :reviewimg="reviewimg6"
          :nameOnReview="nameOnReview6"
          :textOnReview="textOnReview6"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Review from "./Review.vue";
export default {
  data: function() {
    return {
      reviewimg1: require("../../assets/swimmingBoy.png"),
      reviewimg2: require("../../assets/swimmingBoy.png"),
      reviewimg3: require("../../assets/swimmingBoy.png"),
      reviewimg4: require("../../assets/swimmingBoy.png"),
      reviewimg5: require("../../assets/swimmingBoy.png"),
      reviewimg6: require("../../assets/swimmingBoy.png"),
      nameOnReview1: "Jan Nowak",
      nameOnReview2: "Jan Nowak",
      nameOnReview3: "Jan Nowak",
      nameOnReview4: "Jan Nowak",
      nameOnReview5: "Jan Nowak",
      nameOnReview6: "Jan Nowak",
      textOnReview1:
        "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna consetetur sadipscing elitr",
      textOnReview2:
        "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna consetetur sadipscing elitr",
      textOnReview3:
        "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna consetetur sadipscing elitr",
      textOnReview4:
        "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna consetetur sadipscing elitr",
      textOnReview5:
        "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna consetetur sadipscing elitr",
      textOnReview6:
        "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna consetetur sadipscing elitr"
    };
  },
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
    color: #2d3681;
  }
  > p {
    width: 80%;
    max-width: 600px;
    margin: 0 auto 50px;
    text-align: justify;
  }
}
</style>