<template>
  <footer> 
    <div class="footer-top">
      <div class="logo-container">
        <img src="../assets/img/logo_footer.png" alt="Avada image logo">
      </div>
      <div class="burger-menu-container">
        <i class="fas fa-bars fa-2x"></i>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="logo-container">
        <img src="../assets/img/logo_footer.png" alt="Avada image logo">
      </div>
      <div class="burger-menu-container">
        <i class="fas fa-bars fa-2x"></i>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Header",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/Variables.scss";
  footer {
    height: 180px;
    text-align: center;
    
  
    .footer-top {
      padding: 20px;
      height: 120px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      background-color: $brand_secondary_color;
    }

    .footer-bottom {
      padding: 20px;
      height: 100px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      background-color: $brand_tertiary_color;
    }
  }

  .logo-container {
    height: 50px;
  }
  .burger-menu-container {
    color: white;
  }

  button {
    margin: 10px;
  }
</style>
