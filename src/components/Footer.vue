<template>
  <!-- start footer -->
  <footer> 
    <!-- start footer top -->
    <div class="footer-top">
      <div class="logo-container">
        <img src="../assets/img/logo_footer.png" alt="Avada image logo">
      </div>
      <div>
        <ul class="list-container common-text-medium">
          <li v-for="(linkFooter, index) in linksFooter" :key="index" :class="{ current: linkFooter.current }">
            <a :href="linkFooter.url">{{ linkFooter.text }}</a>
          </li>
        </ul>
      </div>
    </div>
    <!-- end footer top -->
    <!-- start bottom footer -->
    <div class="footer-bottom">
      <!-- start first list -->
      <div class="footer-bottom-first-list">
        <ul class="list-container common-text-small">
          <li>&copy; Copyright 2012 - 2021 |</li>
          <li> AVADA THEME BY THEMEFUSION |</li>
          <li> ALL RIGHT RESERVED |</li>
          <li> POWERED BY WORDPRESS</li>
        </ul>
      </div>
      <!-- end first list -->
      <!-- start second list -->
      <div>
        <ul class="list-container">
          <li class="icon-container"><i class="fab fa-twitter fa-xs"></i></li>
          <li class="icon-container"><i class="fab fa-facebook fa-xs"></i></li>
          <li class="icon-container"><i class="fab fa-instagram fa-xs"></i></li>
          <li class="icon-container"><i class="fab fa-youtube fa-xs"></i></li>
        </ul>
      </div>
      <!-- end second list -->  
    </div>
    <!-- end footer bottom -->
    <div class="chevron-container">
      <span class="chevron-icon-container">
        <i class="fas fa-chevron-up"></i>
      </span>
    </div>
  </footer>
  <!-- end footer -->
</template>

<script>
export default {
  name: "Header",
  props: ['linksFooter'],
  data: function() {
    return {
    };
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  // IMPORT AREA
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
    cursor: pointer;
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

  li {
    &.current {
      color: white;
    }
  }
</style>
