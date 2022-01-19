<template>
<div>
  <header id="Home" :class="{hide:colorfull}"> 
    <!-- start menu closed -->
    <div class="menuclosed">
      <div class="header-top">
        <div class="logo-container">
          <img src="../assets/img/avada-music-logo.png" alt="Avada image logo">
        </div>
        <div class="burger-menu-container">
          <i v-on:click="colorfull=!colorfull" class="fas fa-bars fa-2x"></i>
        </div>
      </div>
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
    </div>
  </header>
    <!-- end menu closed -->
    <!-- start menu closed -->
  <div :class="{show:colorfull}" class="headeropen">
    <div class="menuopen">
      <div class="header-top">
        <div class="logo-container">
          <img src="../assets/img/avada-music-logo.png" alt="Avada image logo">
        </div>
        <div  class="burger-menu-container">
          <i v-on:click="colorfull=!colorfull" class="fas fa-times"></i>
        </div>
      </div>
      <div class="header-bottom-closed">
        <ul>
          <li>Home</li>
          <li>Meet the band</li>
          <li>Live dates</li>
          <li>Latest news</li>
          <li>Albums</li>
          <li>Fans</li>
        </ul>
      </div>
    </div>
  </div>
    <!-- end menu closed -->
</div>
  
</template>

<script>
export default {
  name: "Header",
  data() {
        return {
            colorfull:false
        }
    }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
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

  .headeropen {
    height: 600px;
    padding: 20px;
    text-align: center;
    background-color: #ec4958;;
    line-height: 80px;
    font-size: 25px;
    display: none;
  ;

  
    .header-top {
      height: 50px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
  }

  .overlay {
    display: block;
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

  .hide {
    display:none;
  }

  .show {
    display:block;
  }

  
  
</style>
