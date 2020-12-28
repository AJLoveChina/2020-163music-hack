<template>
  <div class="homepage">
    <img src="../assets/jietu/8.jpg" alt="">

    <customInput :x="40" :y="536 + 10" placeholder="夜深了" style="font-size:35px;font-weight: bold;color:white;"></customInput>
    <customInput :x="40" :y="580 + 30 + 10" placeholder="8月2日 04:55， 你还在听着陈炳龙的" style="color:white;"></customInput>
    <customInput :x="40" :y="605 + 35 + 10" placeholder="《白羊》" style="font-size: 21px;color:white;"></customInput>


    <customInput :x="40" :y="605 + 75" placeholder="这一年，有35个不想睡的夜晚" style="text-align: right;width:80%;color:white;" :override="true"></customInput>
    <customInput :x="40" :y="630 + 75" placeholder="有音乐陪你度过" style="text-align: right;width:80%;color:white;"     :override="true"></customInput>

  </div>
</template>

<script>
  import customInput from './input.vue'
export default {
  name: 'Page8',
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
