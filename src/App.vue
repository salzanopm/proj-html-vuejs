<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    Header,
  },
};
</script>

<style lang="scss">
  // import general style settings
  @import './style/Generals.scss';
  // import style variables
   @import './style/Variables.scss';
   
</style>
