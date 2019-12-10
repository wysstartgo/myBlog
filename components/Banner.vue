<template>
  <el-row class="banner" :gutter="0">
    <el-col class="leftBanner" :xs="16" :sm="16" :md="16" :lg="16">
      <el-carousel :interval="5000" height="400px">
        <el-carousel-item class="leftBannerContent">
          <a href="/">
            <img src="../static/img/3.jpg"/>
            <p>
              故不积跬步，无以至千里；不积小流，无以成江海。
            </p>
          </a>
<!--          <div>-->
<!--          </div>-->
        </el-carousel-item>
        <el-carousel-item class="leftBannerContent">
          <a href="/">
            <img src="../static/img/7.jpg"/>
            <p>
              故不积跬步，无以至千里；不积小流，无以成江海。
            </p>
          </a>
<!--          <div>-->
<!--          </div>-->
        </el-carousel-item>
        <el-carousel-item class="leftBannerContent">
          <a href="/">
            <img src="../static/img/10.jpg"/>
            <p>
              故不积跬步，无以至千里；不积小流，无以成江海。
            </p>
          </a>
          <!--          <div>-->
          <!--          </div>-->
        </el-carousel-item>
        <el-carousel-item class="leftBannerContent">
          <a href="/">
            <img src="../static/img/11.jpg"/>
            <p>
              故不积跬步，无以至千里；不积小流，无以成江海。
            </p>
          </a>
          <!--          <div>-->
          <!--          </div>-->
        </el-carousel-item>
        <el-carousel-item class="leftBannerContent">
          <a href="/">
            <img src="../static/img/12.jpg"/>
            <p>
              故不积跬步，无以至千里；不积小流，无以成江海。
            </p>
          </a>
          <!--          <div>-->
          <!--          </div>-->
        </el-carousel-item>
      </el-carousel>
    </el-col>
    <el-col class="rightBanner" :xs="8" :sm="8" :md="8" :lg="8">
      <el-row class="rightTopBanner">
          <div class="banner-img">
          <a href="/">
            <img src="../static/img/8.jpg"/>
            <div>
              <p>
                故不积跬步，无以至千里；不积小流，无以成江海。
              </p>
            </div>
          </a>
        </div>
      </el-row>
      <el-row class="rightBottomBanner">
          <div class="banner-img">
          <a href="/">
            <img src="../static/img/2.jpg"/>
            <div>
              <p>
                故不积跬步，无以至千里；不积小流，无以成江海。
              </p>
            </div>
          </a>
        </div>
      </el-row>
    </el-col>
  </el-row>

</template>

<script>
  import 'element-ui/lib/theme-chalk/display.css';
    export default {
        name: "Banner"
    }
</script>

<style scoped>
  /*.banner {*/
  /*  box-sizing: border-box;*/
  /*}*/
  .banner {
    margin: 0;
    padding: 0;
    /*padding: 0;*/
    width: 100%;
    height: auto;
  }
  .leftBanner {
    padding: 10px;
  }
  .rightBanner {
    padding: 10px;
  }
  .leftBanner .leftBannerContent img{
    min-width: 100%;
    height: 400px;
  }
  .rightBanner .banner-img {
    height: 190px;
    position: relative;
  }
  .rightBanner .banner-img img{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
  .rightBanner .banner-img div {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 50%;
    color: #fff;
    font-size: 16px;
    line-height: 25px;
    background: linear-gradient(0deg,rgba(0,0,0,.8),transparent);
  }
  .rightBanner .banner-img div p {
    padding: 0 20px;
    position: absolute;
    bottom: 10px;
    left: 0;
  }
  .rightBottomBanner {
    margin-top: 20px;
  }
  /*.rightBanner .el-row {*/
  /*  padding: 10px;*/
  /*}*/

</style>
