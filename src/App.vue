<template>
  <div id="app">
    <Controls id="home" />
    <Landing />
    <Boxes />
    <About id="section0" />
    <Trainers id="section2" />
    <Skills />
    <Reviews />
    <Contact id="section1" />
    <FooterComponent />
  </div>
</template>

<script>
import Controls from "./components/Navbar/Controls.vue";
import Landing from "./components/LandingPage/Landing.vue";
import Boxes from "./components/BoxSection/Boxes.vue";
import About from "./components/AboutUs/About.vue";
import Trainers from "./components/TrainersSection/Trainers.vue";
import Skills from "./components/SkillsSection/Skills.vue";
import Reviews from "./components/CustomerReviews/Reviews.vue";
import Contact from "./components/ContactSection/Contact.vue";
import FooterComponent from "./components/Footer/Footer.vue";

export default {
  name: "App",
  components: {
    Controls,
    Landing,
    Boxes,
    About,
    Trainers,
    Skills,
    Reviews,
    Contact,
    FooterComponent
  }
};
</script>

<style lang="scss">
#app {
  overflow-x: hidden;
}
html {
  scroll-behavior: smooth;
}
</style>
