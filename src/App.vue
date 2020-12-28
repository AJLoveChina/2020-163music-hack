<template>
    <div id="app">
        <HomePage2></HomePage2>
    </div>
</template>

<script>
    import HomePage2 from './components/HomePage2.vue'

    export default {
        name: 'App',
        components: {
            HomePage2,
        }
    }
</script>

<style lang="less">
    * {
        margin: 0;
        padding: 0;
    }

    #app {
        font-family: HanHei SC, PingFang SC, Helvetica Neue, Helvetica, sans-serif;
        width: 100%;
        height: 100%;
        position: relative;
        overflow: hidden;
    }


</style>
