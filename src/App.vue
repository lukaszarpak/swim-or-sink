<template>
  <div id="app">
    <Controls />
    <Landing />
    <Boxes />
    <About />
    <Skills />
    <Reviews />
    <Contact />
    <FooterComponent />
  </div>
</template>

<script>
import Controls from "./components/Navbar/Controls.vue";
import Landing from "./components/LandingPage/Landing.vue";
import Boxes from "./components/BoxSection/Boxes.vue";
import About from "./components/AboutUs/About.vue";
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
</style>
