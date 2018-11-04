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
          <el-input
            v-model="searchContent"
            placeholder="搜索商家或地点"
            @focus="searchFocus"
            @blur="searchBlur"/>
          <button class="el-button el-button--primary"><i class="el-icon-search"/></button>
          <dl
            v-if="isHotPlace"
            class="hotPlace">
            <dt>热门搜索</dt>
            <dd
              v-for="(item, idx) in hotPlace"
              :key="idx"
              @click="selectHot">{{ item }}</dd>
          </dl>
          <dl
            v-if="isSearchList"
            class="searchList">
            <dd
              v-for="(item, idx) in searchList"
              :key="idx"
              @click="selectSearch">{{ item }}</dd>
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
        class="right">
        <ul class="security">
          <li><i class="refund"/><p class="txt">随时退</p></li>
          <li><i class="single"/><p class="txt">不满意免单</p></li>
          <li><i class="overdue"/><p class="txt">过期退</p></li>
        </ul>
      </el-col>
    </el-row>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        searchContent: '',
        isFocus: false,
        hotPlace: ['重庆火锅','阿上阿上','关东煮','麻辣小龙虾'],
        searchList: ['干锅鸭头','艾品牛排','羊肉烩面','牛肉蒸饺']
      }
    },
    computed: {
      isHotPlace: function () {
        return this.isFocus && !this.searchContent
      },
      isSearchList: function () {
        return this.isFocus && this.searchContent
      }
    },
    methods: {
      searchFocus: function() {
        this.isFocus = true;
      },
      searchBlur: function () {
        setTimeout(() => {
          this.isFocus = false;
        }, 150)
      },
      selectHot: function () {
        console.log('click host')
      },
      selectSearch: function () {
        console.log('click search')
      }
    }
  }
</script>

<style lang="scss">
@import "@/assets/css/public/header/search.scss";
</style>
