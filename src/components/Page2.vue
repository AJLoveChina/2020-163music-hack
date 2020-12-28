<template>
  <div class="homepage">
    <img src="../assets/jietu/2.jpg" alt="">

    <customInput :x="40" :y="536 + 10" placeholder="2020年，你一共听了" style="line-height: 25px;color:#583d3a;"></customInput>


    <customInput :x="40" :y="580 + 10" placeholder="999小时" style="color:#583d3a; font-size:47px;font-weight: bold;"></customInput>
    <customInput :x="40" :y="630 + 10" placeholder="3956首歌" style="color:#583d3a;font-size:47px;font-weight: bold;"></customInput>


    <customInput :x="40" :y="670 + 40" placeholder="有音乐的每一天" style="line-height: 25px;color:#583d3a;"></customInput>
    <customInput :x="40" :y="700 + 40" placeholder="都会有惊奇的际遇" style="line-height: 25px;color:#583d3a;"></customInput>


  </div>
</template>

<script>
  import customInput from './input.vue'
export default {
  name: 'Page2',
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
