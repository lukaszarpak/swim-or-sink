<template>
  <div class="col-8 col-sm-7 col-md-5 col-lg-3 mx-auto mb-5 sheets">
    <img :src="skillimg" alt="Photo not loaded" />
    <h3>{{textOnSkill}}</h3>
    <p>{{ textOnSkillBottom }}</p>
  </div>
</template>

<script>
export default {
  props: {
    skillimg: String,
    textOnSkill: String,
    textOnSkillBottom: String
  }
};
</script>

<style lang="scss" scoped>
.sheets {
  border: 5px solid #2fc0df;
  border-radius: 30px;
  color: black;
  background-color: #fff;

  > img {
    width: 70%;
    margin: 35px 20px 30px;
  }
  > h3 {
    color: #102c4f;
    margin-bottom: 20px;
  }
  > p {
    text-align: justify;
    margin-bottom: 40px;
  }
}
</style>