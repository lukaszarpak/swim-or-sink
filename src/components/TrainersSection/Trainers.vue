<template>
  <div class="wrap">
    <h2>Nasi Trenerzy</h2>
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren.</p>
    <div class="container mx-auto">
      <div class="row">
        <Trainer
        :trainerPhoto="trainerPhoto1"
        :trainerName="trainerName1"
        :trainerDescription="trainerDescription1"
        />
        <Trainer
        :trainerPhoto="trainerPhoto2"
        :trainerName="trainerName2"
        :trainerDescription="trainerDescription2"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Trainer from './Trainer.vue';
export default {
  data: () => ({
      trainerPhoto1: require("../../assets/KubaSOS.jpg"),
      trainerPhoto2: require("../../assets/KamilSOS.jpg"),
      trainerName1: "Jakub Sobala",
      trainerName2: "Kamil Szulik",
      trainerDescription1: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren.",
      trainerDescription2: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren.",
 }),
 components: {
   Trainer,
 }
};
</script>

<style lang="scss" scoped>
.wrap {
  background:rgba(16, 44, 79, 1);
  text-align: center;
  color: #fff;
  padding: 100px 0 0 0;
  > h2 {
    margin-bottom: 30px;
  }
  > p {
    width: 80%;
    max-width: 600px;
    margin: 0 auto 50px;
    text-align: justify;
  }
}
</style>
