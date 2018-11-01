<template>
  <div class="m-nav">
    <ul class="nav">
      <li class="list">
        <nuxt-link to="/">我的美团</nuxt-link>
        <dl>
          <dd>
            <nuxt-link to="/">我的订单</nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/">我的收藏</nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/">抵用券</nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/">账户设置</nuxt-link>
          </dd>
        </dl>
      </li>
      <li>
        <nuxt-link to="/">手机APP</nuxt-link>
      </li>
      <li class="list bd">
        <nuxt-link to="/">商家中心</nuxt-link>
        <dl>
          <dd>
            <nuxt-link to="/">登录商家中心</nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/">我想合作</nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/">免费手机开店</nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/">商家申请开票</nuxt-link>
          </dd>
        </dl>
      </li>
      <li class="list site">
        <nuxt-link to="/">网站导航</nuxt-link>
        <div class="subContainer">
          <dl class="hotel">
            <dt>酒店</dt>
            <dd>国际机票</dd>
            <dd>自驾旅游</dd>
            <dd>国际机票</dd>
            <dd>自驾旅游</dd>
            <dd>国际机票</dd>
            <dd>自驾旅游</dd>
            <dd>国际机票</dd>
            <dd>自驾旅游</dd>
            <dd>国际机票</dd>
            <dd>自驾旅游</dd>
            <dd>国际机票</dd>
            <dd>自驾旅游</dd>
          </dl>
          <dl class="food">
            <dt>美食</dt>
            <dd>特色小吃</dd>
            <dd>自助大餐</dd>
            <dd>特色小吃</dd>
            <dd>自助大餐</dd>
          </dl>
          <dl class="movie">
            <dt>电影</dt>
            <dd>欧美大片</dd>
            <dd>正在热影</dd>
            <dd>怀旧精典</dd>
            <dd>怀旧精典</dd>
            <dd>怀旧精典</dd>
          </dl>
          <dl class="app">
            <dt>手机应用</dt>
            <dd>
              <a
                href="https://i.meituan.com/mobile/down/meituan"
                target="_blank"><img
                  class="appicon"
                  src="//s0.meituan.net/bs/fe-web-meituan/e5eeaef/img/appicons/meituan.png"
                  title="美团app"
                  alt="美团app"></a>
            </dd>
            <dd>
              <a
                href="https://www.dianping.com/events/m/index.htm"
                target="_blank"><img
                  class="appicon"
                  src="//s1.meituan.net/bs/fe-web-meituan/404d350/img/appicons/dianping.png"
                  title="点评app"
                  alt="点评app"></a>
            </dd>
          </dl>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
  }
</script>
