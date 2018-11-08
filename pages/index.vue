<template>
  <div class="page-index">
    <el-row>
      <el-col :span="5">
        <my-menu/>
      </el-col>
      <el-col :span="19">2</el-col>
    </el-row>
    <el-row>
      <el-col :span="24">3</el-col>
    </el-row>
  </div>
</template>

<script>
  import MyMenu from '@/components/index/menu.vue'

  export default {
    components: {
      MyMenu
    }
  }
</script>

<style lang="scss">
  @import "@/assets/css/index/index.scss";
</style>
