<template>
  <header> 
    <div class="header-top">
      <div class="logo-container">
        <img src="../assets/img/avada-music-logo.png" alt="Avada image logo">
      </div>
      <div class="burger-menu-container">
        <i class="fas fa-bars fa-2x"></i>
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
  </header>
</template>

<script>
export default {
  name: "Header",
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

  .logo-container {
    height: 100%;
  }

  .burger-menu-container {
    color: white;
  }

  button {
    margin: 10px;
  }
</style>
