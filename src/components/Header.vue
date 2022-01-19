<template>
  <!-- start menu wrapper -->
  <div class="menu-wrapper">
    <!-- start header with static menu -->
    <header id="Home" :class="{hide:active}"> 
      <!-- start menu closed -->
      <div class="menuclosed">
        <!-- start top menu -->
        <div class="header-top">
          <div class="logo-container">
            <img src="../assets/img/avada-music-logo.png" alt="Avada image logo">
          </div>
          <div class="burger-menu-container">
            <i v-on:click="active=!active" class="fas fa-bars fa-2x"></i>
          </div>
        </div>
        <!-- end top menu -->
        <!-- start bottom menu -->
        <div class="header-bottom">
          <div class="header-bottom-title">
            <h1>Untold Stories</h1>
            <h4>There is a untold story behind every favorite song</h4>
          </div>
          <div class="header-bottom-buttons">
            <button class="button-red">Latest album</button>
            <button class="button-transparent">Live dates</button>
          </div>
        </div>
        <!-- end bottom menu -->
      </div>
      <!-- end menu closed -->
    </header>
    <!-- start header with static menu -->
    <!-- start second header menu open -->
    <div :class="{show:active}" class="headeropen">
      <!-- start menu open -->
      <div class="menuopen">
        <!-- start header top -->
        <div class="header-top">
          <div class="logo-container">
            <img src="../assets/img/avada-music-logo.png" alt="Avada image logo">
          </div>
          <div  class="burger-menu-container">
            <i v-on:click="active=!active" class="fas fa-times fa-lg"></i>
          </div>
        </div>
        <!-- end header top -->
        <!-- start header bottom -->
        <div class="header-bottom-closed">
          <ul>
            <li v-for="(linkHeader, index) in linksHeader" :key="index" :class="{ current: linkHeader.current }">
              <a :href="linkHeader.url">{{ linkHeader.text }}</a>
            </li>
            <!-- <li><a href="#">Home</a></li>
            <li><a href="#meet-the-band">Meet the band</a></li>
            <li><a href="#live-dates">Live dates</a></li>
            <li><a href="#latest-news">Latest news</a></li>
            <li><a href="#">Albums</a></li>
            <li><a href="#">Fans</a></li> -->
          </ul>
        </div>
        <!-- end header bottom -->
      </div>
      <!-- end menu open -->
    </div>
    <!-- start second header menu open -->
  </div>
  <!-- end menu wrapper -->
</template>

<script>
export default {
  name: "Header",
  props: ['linksHeader'],
  data() {
    return {
        active:false
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  // first header
  header {
    height: 600px;
    padding: 20px;
    text-align: center;
    background-image: url('../assets/img/home_slider.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  
    .header-top {
      height: 50px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
  }

  .logo-container {
    height: 100%;
  }

  .burger-menu-container {
    color: white;
  }

  button {
    margin: 10px;
  }

  // second header
  .headeropen {
    height: 600px;
    padding: 20px;
    text-align: center;
    background-color: #ec4958;;
    line-height: 80px;
    font-size: 25px;
    display: none;
  
    .header-top {
      height: 50px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
  }

  // active classes
  .hide {
    display:none;
  }

  .show {
    display:block;
  }
</style>
