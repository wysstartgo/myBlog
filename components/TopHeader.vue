<template>
<header class="appHead">
  <el-row class="nav" :gutter="0">
    <el-col class="navBar" :xs="22" :sm="22" :md="22" :lg="16">
      <div class="logoDiv">
        <a href="/"><img src="@/assets/logo.png" alt></a>
      </div>
      <div class="leftMenu">
        <el-menu :router=true menu-trigger="click" active-text-color="#5FB878" :default-active="activeIndex"
                 mode="horizontal">
          <el-menu-item index="/">技术</el-menu-item>
          <el-menu-item>java</el-menu-item>
          <el-menu-item>唐诗</el-menu-item>
          <el-menu-item>宋词</el-menu-item> <el-menu-item>java</el-menu-item>
          <el-menu-item>唐诗</el-menu-item>
          <el-menu-item>宋词</el-menu-item> <el-menu-item>java</el-menu-item>
          <el-menu-item>唐诗</el-menu-item>
          <el-menu-item>宋词</el-menu-item> <el-menu-item>java</el-menu-item>
          <el-menu-item>唐诗</el-menu-item>
          <el-menu-item>宋词</el-menu-item>
        </el-menu>
      </div>
    </el-col>
    <el-col class="rightMenu" :xs="2" :sm="2" :md="2" :lg="8">
      <div v-if="!userinfo">
        <a href="/user/login">
          <el-button
            type="primary"
            icon="el-icon-user"
            id="login"
            style="margin-right: 10px"
          >登陆</el-button>
        </a>
        <a href="/user/register">
          <el-button type="primary" icon="el-icon-edit" id="register">注册</el-button>
        </a>
      </div>

      <div v-else class="nav-avatar">
        <el-menu class="el-menu-demo" mode="horizontal">
          <el-submenu index="2">
            <template slot="title">
              <a href="javascript:;">
                <img src="@/assets/logo.png">
<!--                <img :src="avatar" v-if="avatar" class="layui-nav-img" />-->
              </a>
            </template>
            <el-menu-item index="2-3" class="el-icon-position" @click="logout">退出</el-menu-item>
          </el-submenu>
        </el-menu>
      </div>
    </el-col>
  </el-row>
</header>
</template>

<script>
    export default {
      name: "TopHeader",
      data() {
        return {
          activeIndex: '/',
          userinfo: {}
        };
      },
      methods: {
        handleClick(tab, event) {
          console.log(tab, event);
        },
        logout() {
          
        }
      }
    }
</script>

<style scoped>
.navBar {
  display: flex;
}
.leftMenu {
  padding-left: 50px;
}
.logoDiv img{
  width: 100%;
  max-width: 100px;
}
.el-menu.el-menu--horizontal{
  border-bottom: none;
}
</style>
