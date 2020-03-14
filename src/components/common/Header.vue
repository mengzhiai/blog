<template>
<div class="header">
  <ul class="flex">
    <li v-for="(item, i) in navList" :key="i">{{item.name}}</li>
  </ul>
</div>
</template>

<script>
export default {
  data() {
    return {
      navList: [{
        name: '首页'
      }, {
        name: '前端'
      }, {
        name: '数据库'
      }, {
        name: '技术交流'
      }, {
        name: '关于我们'
      }, {
        name: '留言'
      }]
    };
  }
};
</script>
<style lang="scss" scoped>
// @import '@/styles/common.scss';
.header{
  color: #fff;
  // background-color: #409EFF;
  background-color: $theme-color;
  ul{
    li{
      font-size: $fontSize;
    }
  }
}
</style>
