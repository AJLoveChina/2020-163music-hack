<template>
  <div class="input" ref="wrap" :style="{top:`${y}px`, left:`${x}px`}">
    <div class="placeholder" v-if="input ==='' || override" v-text="(override && input !== '') ? input : placeholder"></div>
    <input ref='input' type="text" v-model="input" @input="jisuan">
  </div>
</template>

<script>
export default {
  name: 'customInput',
  props: {
    x:Number,
    y:Number,
    placeholder:String,
    year: Object,
    override: Boolean,
  },
  data() {
    return {
      input:""
    }
  },
  mounted() {
    if (this.override) {
      this.$refs.input.style.color = 'transparent'
    } else {
      this.$refs.input.style.color = this.$refs.wrap.style.color;
    }
  },
  methods: {
    jisuan() {
      try {
        let year = /\d\s*年/.exec(this.input)[0].replace(/[^\d]/gi, "")
        this.year.num = year;
      } catch (e) {
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
  .input{
    position: absolute;
    width:100%;


    .placeholder{
      position: absolute;
      top:0;left:0;
      width:100%;
    }

    input {
      position: absolute;
      top:0;left:0;
      width:100%;
      background: transparent;
      border:none;
      outline:none;
    }
  }
</style>
