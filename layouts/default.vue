<template>
  <div id="app" class="blog-index">
    <top-header :activeIndex="activeIndex"></top-header>
    <div>
      <nuxt />
    </div>
  </div>
</template>

<style>

</style>
<script>
  import TopHeader from "../components/TopHeader";
  export default {
    components: {TopHeader},
    data: {
      activeIndex: "/"
    }
  }
</script>
