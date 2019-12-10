<template>
<el-row class="articlesAndSlide" :gutter="20">
  <el-col :span="17" class="articles">
      <ArticleList></ArticleList>
  </el-col>
  <el-col :span="7">
      <SlideContent></SlideContent>
  </el-col>
</el-row>
</template>

<script>
    import ArticleList from "./ArticleList";
    import SlideContent from "./SlideContent";
    export default {
        name: "MainArticleContent",
      components: {SlideContent, ArticleList}
    }
</script>

<style scoped>
.articlesAndSlide {
  padding: 0 30px;
  margin-bottom: 30px;
}
</style>
