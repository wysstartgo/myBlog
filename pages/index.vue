<template>
  <div class="container">
    <transition name="fade">
      <Loading v-if="isLoading"></Loading>
    </transition>
    <Banner></Banner>
    <MainContent></MainContent>
  </div>
</template>

<script>

import Loading from "../components/Loading";
import Banner from "../components/Banner";
import MainContent from "../components/MainArticleContent";
export default {
  name: "latestRecommendStrategyArticle",
  components: {MainContent, Banner, Loading},
  data(){
    return {
      isLoading:false
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  /*min-height: 100vh;*/
  /*display: flex;*/
  /*justify-content: center;*/
  /*align-items: center;*/
  /*text-align: center;*/
  /*background: linear-gradient(45deg,#222428,#444856);*/
}
/*.el-row {*/
/*  margin-bottom: 20px;*/

/*  &:last-child {*/
/*    margin-bottom: 0;*/
/*  }*/
/*}*/



</style>
