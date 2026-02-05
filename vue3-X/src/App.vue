
<template>

    <Person></Person>
</template>

<script lang="ts">
 //脚本
 import Person from './components/Prseon.vue'
 export default {
    name: 'App',//组件的名称
    components: {Person},//注册组件
 }
 
</script>
 
<style >
    /* 样式 */
    .app {
        box-shadow: 0 0 10px 10px rgba(0, 0, 0, 0.1);
        background-color: rgb(18, 75, 182);
        padding: 20px;
        border-radius: 8px;
    }
</style>
