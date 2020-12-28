<template>
  <div class="homepage">
    <img src="../assets/jietu/1.jpg" alt="">
    <customInput :x="40" :y="426" placeholder="Hi~" style="font-size: 32px;
    color: #583d3a;
        font-weight: bold;
    line-height: 35px;"></customInput>

    <div class="year">{{year.num}}</div>

    <customInput :x="40" :y="462" :year="year" :placeholder="`我们在一起${year.num}年啦!`" style="font-size: 32px;
    color: #583d3a;
    -webkit-tap-highlight-color:rgba(0, 0, 0, 0);
    font-weight: bold;
    line-height: 35px;"></customInput>


    <customInput :x="40" :y="520 + 10" placeholder="2015年02月02日" style="line-height: 25px;color:#583d3a;"></customInput>
    <customInput :x="40" :y="545 + 10" placeholder="第一次遇见你" style="line-height: 25px;color:#583d3a;"></customInput>



    <customInput :x="40" :y="580 + 20" placeholder="Pink/Nate RUess的" style="line-height: 25px;color:#583d3a;"></customInput>
    <customInput :x="40" :y="605 + 20" placeholder="<Just Give me a Reason>" style="line-height: 25px;color:#583d3a;font-weight: bold;"></customInput>
    <customInput :x="40" :y="630 + 20" placeholder="是你听的第一首歌" style="line-height: 25px;color:#583d3a;"></customInput>


  </div>
</template>

<script>
  import customInput from './input.vue'
export default {
  name: 'HomePage2',
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
