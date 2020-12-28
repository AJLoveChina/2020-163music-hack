<template>
  <div class="homepage">
    <img src="../assets/jietu/0.jpg" alt="">

    <div class="title">网抑云音乐<br> 2020年度回顾 <br> 私人订制</div>
    <div class="sub-title">
      idea by lwmao && 何烫头 <br><br>
      created by <a href="https://zhihu.com/people/AJLoveChina" target="_blank">霸都丶傲天</a> <br><br>

      点击最底部按钮 即可切换页面

    </div>
  </div>
</template>

<script>
  import customInput from './input.vue'
export default {
  name: 'Page0',
  props: {
  },
  components: {
    customInput,
  },
  data() {
    return {
      year:{
        num:6
      },
    }
  },
  mounted() {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
  .title {
    position: absolute;
    width:100%;
    top:50px;
    font-size: 40px;
    font-weight: bold;
    text-align: center;
    padding: 0 20px;
  }
  .sub-title{
    position: absolute;
    width:100%;
    top:240px;
    font-size: 12px;
    color:#333;
    text-align: center;
  }
</style>
