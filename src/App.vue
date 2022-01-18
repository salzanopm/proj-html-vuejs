<template>
  <div id="app">
    <Header />
    <FirstSection />
    <SecondSection />
    <ButtonBig />
    <ThirdSection />
    <FourthSection />
    <ButtonBig2 />
    <Footer :links="linksArray" />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import FirstSection from "./components/FirstSection.vue";
import SecondSection from "./components/SecondSection.vue";
import ButtonBig from "./components/ButtonBig.vue";
import ThirdSection from "./components/ThirdSection.vue";
import FourthSection from "./components/FourthSection.vue";
import ButtonBig2 from "./components/ButtonBig2.vue";
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
    ButtonBig2,
    Footer,
  },
  data: function() {
    return {
      linksArray: [
        {
          text: 'Home',
          url: '#Home',
          current: true,
        },
        {
          text: 'Meet the band',
          url: '#meet-the-band',
          current: false,
        },
        {
          text: 'Live dates',
          url: '#live-dates',
          current: false,
        },
        {
          text: 'Latest News',
          url: '#latest-news',
          current: false,
        },
        {
          text: 'Abums',
          url: '#',
          current: false,
        },
        {
          text: 'Fans',
          url: '#',
          current: false,
        }
      ],
    }
  }
};
</script>

<style lang="scss">
  // import general style settings
  @import './style/Generals';
  // import style variables
   @import './style/Variables';
   
</style>
