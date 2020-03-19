<template>
  <div class="wrap">
    <h2>Nasze specjalności</h2>
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren.</p>
    <div class="container mx-auto">
      <div class="row">
        <Skill
          :skillimg="skillimg1"
          :textOnSkill="textOnSkill1"
          :textOnSkillBottom="textOnSkillBottom1"
        />
        <Skill
          :skillimg="skillimg2"
          :textOnSkill="textOnSkill2"
          :textOnSkillBottom="textOnSkillBottom2"
        />
        <Skill
          :skillimg="skillimg3"
          :textOnSkill="textOnSkill3"
          :textOnSkillBottom="textOnSkillBottom3"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Skill from "./Skill.vue";
export default {
  name: "Skills",
  data: function() {
    return {
      skillimg1: require("../../assets/skill1.png"),
      skillimg2: require("../../assets/skill2.png"),
      skillimg3: require("../../assets/skill3.png"),
      textOnSkill1: "Początkujący",
      textOnSkill2: "Zaawansowany",
      textOnSkill3: "Sportowiec",
      textOnSkillBottom1:
        "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor",
      textOnSkillBottom2:
        "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor",
      textOnSkillBottom3:
        "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor"
    };
  },
  components: {
    Skill
  }
};
</script>

<style scoped lang="scss">
.wrap {
  background: linear-gradient(
    180deg,
    rgba(16, 44, 79, 1) 0%,
    rgba(33, 75, 124, 1) 80%
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
    text-align: justify;
  }
}
</style>
