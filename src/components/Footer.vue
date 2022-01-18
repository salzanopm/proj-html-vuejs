<template>
  <footer> 
    <div class="footer-top">
      <div class="logo-container">
        <img src="../assets/img/logo_footer.png" alt="Avada image logo">
      </div>
      <div>
        <ul class="list-container">
          <li class="common-text2"><a href="#">1</a></li>
          <li class="common-text2"><a href="#">1</a></li>
          <li class="common-text2"><a href="#">1</a></li>
          <li class="common-text2"><a href="#">1</a></li>
          <li class="common-text2"><a href="#">1</a></li>
          <li class="common-text2"><a href="#">1</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <div>
        <ul class="list-container">
          <li>1</li>
          <li>|</li>
          <li>1</li>
          <li>|</li>
          <li>1</li>
          <li>|</li>
          <li>1</li>
        </ul>
      </div>
      <div>
        <ul class="list-container">
          <li class="icon-container"><i class="fab fa-twitter fa-xs"></i></li>
          <li class="icon-container"><i class="fab fa-facebook fa-xs"></i></li>
          <li class="icon-container"><i class="fab fa-instagram fa-xs"></i></li>
          <li class="icon-container"><i class="fab fa-youtube fa-xs"></i></li>
        </ul>
      </div>
    </div>
    <div class="chevron-container">
      <span class="chevron-icon-container">
        <i class="fas fa-chevron-up"></i>
      </span>
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

  .list-container {
    display: flex;
    flex-direction: row;
  }

  .fab,
  .fas {
    color: $medium_text_color;
  }

  .icon-container {
    height: 30px;
    width: 30px;
    background-color: $brand_secondary_color;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 2px;
  }

  .logo-container {
    height: 50px;
  }

  .chevron-container {
    position: relative;
  }

  .chevron-icon-container {
    height: 25px;
    width: 30px;
    background-color: #323233;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 2px;
    position: absolute; 
    bottom: 5px;
    right: 35px;
  }
</style>
