<template>
  <div id="app" class="blog-index">
    <top-header :activeIndex="activeIndex"></top-header>
<!--    <el-row class="main">-->
<!--      <el-col class="mainContent">-->
<!--      </el-col>-->
<!--    </el-row>-->
    <nuxt />

    <Footer></Footer>
  </div>
</template>

<style>

</style>
<script>
  import TopHeader from "../components/TopHeader";
  import Footer from "../components/Footer";
  export default {
    components: {Footer, TopHeader},
    data() {
      return {
        activeIndex: "/"
      }
    }
  }
</script>
