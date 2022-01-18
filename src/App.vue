<template>
  <div id="app">
    <Header />
    <FirstSection />
    <SecondSection />
    <ButtonBig />
    <ThirdSection />
    <FourthSection />
    <ButtonBig />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import FirstSection from "./components/FirstSection.vue";
import SecondSection from "./components/SecondSection.vue";
import ButtonBig from "./components/ButtonBig.vue";
import ThirdSection from "./components/ThirdSection.vue";
import FourthSection from "./components/FourthSection.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    Header,
    FirstSection,
    SecondSection,
    ButtonBig,
    ThirdSection,
    FourthSection,
    Footer,
  },
};
</script>

<style lang="scss">
  // import general style settings
  @import './style/Generals';
  // import style variables
   @import './style/Variables';
   
</style>
