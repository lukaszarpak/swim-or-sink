<template>
  <div class="wrap">
    <h2>Opinie klientów</h2>
    <p>
      Zachęcamy do zostawienia opinii na temat naszych zajęć na naszej
      <a
        href="https://www.facebook.com/SwimOrSink.SzkolaPlywania/"
        target="_blank"
      >stronie facebookowej</a>.
    </p>
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
      reviewimg1: require("../../assets/reviews/reviewPhoto1.png"),
      reviewimg2: require("../../assets/reviews/reviewPhoto2.png"),
      reviewimg3: require("../../assets/reviews/reviewPhoto3.png"),
      reviewimg4: require("../../assets/reviews/reviewPhoto4.png"),
      reviewimg5: require("../../assets/reviews/reviewPhoto5.png"),
      reviewimg6: require("../../assets/reviews/reviewPhoto6.png"),
      nameOnReview1: "Artur Rozner",
      nameOnReview2: "Kamila Góreczny",
      nameOnReview3: "Gabriel Turczyński",
      nameOnReview4: "Marta Sikorska",
      nameOnReview5: "Katarzyna Mroczkowska",
      nameOnReview6: "Robert Morganti",
      textOnReview1:
        "Zróżnicowane zajęcia, bardzo ciekawe ćwiczenia, indywidualne podejście a efektem tego są szybkie postępy. Gorąco polecam!",
      textOnReview2:
        "Moja osobista opinia byłaby stronnicza, gdyż znam i cenię Kubę od dawna. Za to po wczorajszych zajęciach mogę przekazać opinię swoich dzieci, 13-latki i 7-latka. Są zachwyceni. Szukając szkoły pływania od razu pomyślałam o szkole Kuby i Kamila i nie zawiodłam się.",
      textOnReview3: "Polecam.. profesjonalni trenerzy.",
      textOnReview4:
        "Polecam, mój pięciolatek jest zachwycony. I przede wszystkim rewelacyjne godziny zajęć. Dzięki chłopaki.",
      textOnReview5:
        "Polecam. Moja 6-latka zachwycona pierwszymi zajęciami. Oby tak zostało.",
      textOnReview6: "Super szkoła, ekstra chłopaki, pozdrawiam."
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