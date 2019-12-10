<template>
  <footer class="navFooter hidden-sm-and-down">
    <el-footer class="me-area" >
      <div class="me-footer">
        <router-link to="/" class="footer-logo"><img src="../assets/logo.png"></router-link>&nbsp;&nbsp;&nbsp;&nbsp;
        <i style="font-size: 5px;font-family: 'Apple Color Emoji';font-weight: bold;color:#fff">点 滴 分 享</i>&nbsp;&nbsp;&nbsp;&nbsp;
        <a href="http://beian.miitbeian.gov.cn" style="font-size: 5px;font-family: 'Apple Color Emoji';font-weight: bold;color:#fff;text-decoration: none;">&nbsp;&nbsp;&nbsp;&nbsp;浙ICP备19047566号</a>
      </div>
    </el-footer>
  </footer>
</template>

<script>
    export default {
        name: "Footer"

    }
</script>

<style scoped>
  .navFooter {
    padding-top: 70px;
  }
  .me-area {
    box-sizing: border-box;
    /*padding-top: 70px;*/
    height: auto !important;
    background: linear-gradient(45deg,#222428,#444856);
    text-align: center;
  }
  .me-footer {
    box-sizing: border-box;
    text-align: center;
    line-height: 60px;
    vertical-align: center;
    font-family: 'Open Sans', sans-serif;
    font-size: 18px;

  }


  .footer-logo {
    display: inline-block;
    vertical-align: middle;
    text-align: center;
  }
  .me-footer img {
    height: 50px;
    width: 72px;
  }
  .footer-logo{
    text-align: center;
  }



</style>
