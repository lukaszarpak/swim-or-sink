<template>
  <div class="col-8 col-md-5 mx-auto mb-5 trainer">
    <img :src="trainerPhoto" alt="Photo not loaded" />
    <h3>{{ trainerName }}</h3>
    <p>{{ trainerDescription }}</p>
  </div>
</template>

<script>
export default {
  props: {
    trainerPhoto: String,
    trainerName: String,
    trainerDescription: String
  }
};
</script>

<style lang="scss" scoped>
.trainer {
  border: 5px solid #2fc0df;
  border-radius: 30px;
  color: black;
  background-color: #fff;

  > img {
    width: 90%;
    margin: 35px auto 30px;
    border-radius: 30px;
  }
  > h3 {
    color: #102c4f;
    margin-bottom: 20px;
  }
  > p {
    text-align: justify;
    margin: 0 auto;
    margin-bottom: 30px;
    width: 90%;
  }
}
</style>