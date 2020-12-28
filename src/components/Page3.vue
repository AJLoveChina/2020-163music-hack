<template>
  <div class="homepage">
    <img src="../assets/jietu/3.jpg" alt="">

    <customInput :x="40" :y="536 + 10" placeholder="春天你最爱" style="font-size:35px;font-weight: bold"></customInput>
    <customInput :x="40" :y="580 + 30 + 10" placeholder="红人馆/红人馆馆长" style=""></customInput>
    <customInput :x="40" :y="605 + 35 + 10" placeholder="《最甜情歌》" style="font-size: 21px"></customInput>


    <customInput :x="40" :y="605 + 75" placeholder="它随春日樱花" style="text-align: right;width:80%" :override="true"></customInput>
    <customInput :x="40" :y="630 + 75" placeholder="一起到来" style="text-align: right;width:80%"     :override="true"></customInput>

  </div>
</template>

<script>
  import customInput from './input.vue'
export default {
  name: 'Page3',
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
