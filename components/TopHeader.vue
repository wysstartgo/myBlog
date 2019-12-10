<template>
<header class="appHead">
  <el-row class="myNav" :gutter="0">
    <el-col class="navLogo" :xs="1" :sm="1" :md="1" :lg="1">
      <div class="logoDiv">
        <a href="/"><img src="@/assets/logo.png" alt></a>
      </div>
    </el-col>
    <el-col class="navName hidden-sm-and-down" :xs="2" :sm="4" :md="4" :lg="2" >
       点 滴 分 享
    </el-col>
    <el-col class="navBar" :xs="19" :sm="9" :md="13" :lg="17">
      <div class="navMenu">
        <el-menu :router=true menu-trigger="click" active-text-color="#5FB878" :default-active="activeIndex"
                 mode="horizontal">
          <el-menu-item index="/">技术</el-menu-item>
          <el-menu-item class="hidden-sm-and-down">java</el-menu-item>
          <el-menu-item>唐诗</el-menu-item>
          <el-menu-item>宋词</el-menu-item>
          <el-menu-item class="hidden-sm-and-down">java</el-menu-item>
        </el-menu>
      </div>
    </el-col>
    <el-col class="rightMenu hidden-sm-and-down" :xs="2" :sm="10" :md="6" :lg="4" >
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
  import 'element-ui/lib/theme-chalk/display.css';

    export default {
      name: "TopHeader",
      data() {
        return {
          activeIndex: '/',
          userinfo: ''
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
/*.myNav:after {*/
/*  content: "";*/
/*  display: block;*/
/*  clear: both;*/
/*}*/
.myNav {
  width: 100%;
  height: 60px;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 99;
  background-color: #fafafa;
  -webkit-box-shadow: 0 2px 10px 0 rgba(0,0,0,.1), 0 1px rgba(66,66,66,.1);
  box-shadow: 0 2px 10px 0 rgba(0,0,0,.1), 0 1px rgba(66,66,66,.1);
  z-index: 99999;
}
.logoDiv {
  text-align: center;
}
.logoDiv img{
  width: 100%;
  max-width: 150px;
}
.rightMenu {
  line-height: 60px;
}
.navName {
  line-height: 60px;
  text-align: center;
  font-family: 华文行楷;
  padding: 0 5px;
}
.el-menu.el-menu--horizontal{
  border-bottom: none;
}
</style>
