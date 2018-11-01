<template>
  <div class="search-panel">
    <el-row class="m-header-searchbar">
      <el-col
        :span="3"
        class="left">
        <img src="//s0.meituan.net/bs/fe-web-meituan/e5eeaef/img/logo.png">
      </el-col>
      <el-col
        :span="15"
        class="center">
        <div class="wrapper">
          <el-input placeholder="搜索商家或地点"/>
          <button class="el-button el-button--primary"><i class="el-icon-search"/></button>
          <dl class="hotPlace">
            <dt>热门搜索</dt>
            <dd>火锅</dd>
            <dd>麻辣烫</dd>
            <dd>小龙虾</dd>
          </dl>
          <dl class="searchList">
            <dd>阿上阿上</dd>
            <dd>干锅鸭头</dd>
            <dd>艾品牛排</dd>
            <dd>羊肉烩面</dd>
            <dd>牛肉蒸饺</dd>
          </dl>
        </div>
        <p class="suggset">
          <a href="#">故宫博物院</a>
          <a href="#">故宫博物院</a>
          <a href="#">故宫博物院</a>
          <a href="#">故宫博物院</a>
        </p>

        <ul class="nav">
          <li>
            <nuxt-link
              to="/"
              class="takeout">美团外卖</nuxt-link>
          </li>
          <li>
            <nuxt-link
              to="/"
              class="takeout">猫眼电影</nuxt-link>
          </li>
          <li>
            <nuxt-link
              to="/"
              class="takeout">民宿/公寓</nuxt-link>
          </li>
          <li>
            <nuxt-link
              to="/"
              class="takeout">商家入驻</nuxt-link>
          </li>
        </ul>
      </el-col>
      <el-col
        :span="6"
        class="right">3</el-col>
    </el-row>
  </div>
</template>

<script>
  export default {
  }
</script>

<style>
@import "@/assets/css/public/header/search.scss";
</style>
