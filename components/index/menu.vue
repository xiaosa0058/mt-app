<template>
  <div class="m-menu">
    <dl class="nav">
      <dt>全部分类</dt>
      <dd
        v-for="(item, idx) in menu"
        :key="idx">
        <i :class="item.type"/>{{ item.name }}<span class="arrow"/>
      </dd>
    </dl>
    <div class="detail">
      <template v-for="(item, idx) in curDetail">
        <h4 :key="idx">{{ item.title }}</h4>
        <span
          v-for="v in item.list"
          :key="v">{{ v }}</span>
      </template>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        kind: '',
        menu: [{
          type: 'food',
          name: '美食',
          child: [{
            title: '中国菜',
            list: ['川菜', '鲁菜', '东北菜', '北京卤煮', '湘菜', '安徽板面', '沙县小吃']
          },{
            title: '西餐',
            list: ['牛排', '沙拉', '汉堡', '薯条', '披萨', '意大利面', '印度薄饼']
          }]
        },{
          type: 'takeout',
          name: '外卖',
          child: [{
            title: '外卖',
            list: ['美团外卖']
          }]
        },{
          type: 'hotel',
          name: '酒店',
          child: [{
            title: '酒店',
            list: ['经济型', '舒适/三星', '高档/四星', '豪华/五星']
          }]
        }]
      }
    },
    computed: {
      curDetail: function() {
        const detail = this.menu.filter(item => item.type === this.kind)[0];
        return detail ? detail.child : [];
      }
    }
  }
</script>
