<template>
  <div class="homepage" :style="{zoom: zoom}">
    <img src="../assets/jietu/1.jpg" alt="">
  </div>
</template>

<script>
export default {
  name: 'HomePage2',
  props: {
    msg: String
  },
  data() {
    return {
      zoom: 1
    }
  },
  mounted() {
    let w = 540;
    let h = 870;

    let ww = window.innerWidth;
    let wh = window.innerHeight;

    let zoom = ww / w;
    this.zoom = zoom;
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
</style>
