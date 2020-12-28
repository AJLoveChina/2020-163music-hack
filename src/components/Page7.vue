<template>
  <div class="homepage">
    <img src="../assets/jietu/7.jpg" alt="">

    <customInput :x="40" :y="536 + 10" placeholder="单曲循环了520次" style="font-size:35px;font-weight: bold"></customInput>
    <customInput :x="40" :y="580 + 30 + 10" placeholder="07月12日，你播放 颜人中 的" style=""></customInput>
    <customInput :x="40" :y="605 + 35 + 10" placeholder="《晚安》" style="font-size: 21px"></customInput>


    <customInput :x="40" :y="605 + 75" placeholder="相信那一天" style="text-align: right;width:80%" :override="true"></customInput>
    <customInput :x="40" :y="630 + 75" placeholder="留在你记忆里的不止是这首歌吧" style="text-align: right;width:80%"     :override="true"></customInput>

  </div>
</template>

<script>
  import customInput from './input.vue'
export default {
  name: 'Page7',
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
  .homepage{
    position: relative;
  }
  .year{
    position: absolute;
    top: -7px;
    left: 328px;
    font-size: 250px;
    font-weight: bold;
    color: white;
    text-shadow: #d4bf4d 0 0 20px;
  }
</style>
