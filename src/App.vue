<template>
    <div id="app" :style="{zoom: zoom}">
        <Page0 v-if="page === 0"></Page0>
        <HomePage2 v-if="page === 1"></HomePage2>
        <Page2 v-if="page === 2"></Page2>
        <Page3 v-if="page === 3"></Page3>
        <Page4 v-if="page === 4"></Page4>
        <Page5 v-if="page === 5"></Page5>
        <Page6 v-if="page === 6"></Page6>
        <Page7 v-if="page === 7"></Page7>
        <Page8 v-if="page === 8"></Page8>

        <div>
            <button class="btn" @click="page--" :disabled="page === 0">上一页</button>
            <button class="btn" @click="page++" :disabled="page === max">下一页</button>
        </div>
    </div>
</template>

<script>
    import HomePage2 from './components/HomePage2.vue'
    import Page0 from './components/Page0.vue'
    import Page2 from './components/Page2.vue'
    import Page3 from './components/Page3.vue'
    import Page4 from './components/Page4.vue'
    import Page5 from './components/Page5.vue'
    import Page6 from './components/Page6.vue'
    import Page7 from './components/Page7.vue'
    import Page8 from './components/Page8.vue'

    export default {
        name: 'App',
        components: {
            HomePage2,
            Page0,
            Page2,
            Page3,
            Page4,
            Page5,
            Page6,
            Page7,
            Page8,
        },
        data() {
            return {
                page:0,
                max:8,
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

<style lang="less">
    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        font-family: Microsoft Yahei;
        font-size: inherit;
        color: inherit;
        font-weight: inherit;
    }

    #app {
        font-family: HanHei SC, PingFang SC, Helvetica Neue, Helvetica, sans-serif;
        width: 100%;
        height: 100%;
        position: relative;
        overflow: hidden;
        color:#583d3a;
        font-size: 16px;

        > div{
          width:100%;
            height: 100%;
        }

        .btn{
            padding:5px;background: #ccc;
            margin:0 10px;
        }
    }


</style>
