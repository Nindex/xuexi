
<template>
  <div class="perseon">
    <h1>姓名：{{ name }}</h1>
    <p>年龄：{{ age }}</p>
    <button @click="changeAge">减少年龄</button>
    <button @click="changeAge1">增加年龄</button>
    <button @click="changeAge2">设置年龄</button>
    <button @click="changeAge3">清空年龄</button>
  </div>
</template>

<script lang="ts">
import { ref } from 'vue'

export default {
  name: 'Perseon',
  setup() {
    // 数据
      let name: string = '张三'
      let age = ref<number>(18)
      // 方法
      function changeAge() {
        age.value--
      }
      function changeAge1() {
        age.value++
      }
      // 方法
      function changeAge2() {
        age.value = 20
      }
      // 方法
      function changeAge3() {
        age.value = 0
      }
      let TEL: string = '13800000000'
    return {name,age,changeAge,changeAge1,changeAge2,changeAge3,TEL}  
  }
}
</script>

<style scoped>
    .perseon {
        box-shadow: 0 0 10px;
        background-color: skyblue;
        padding: 20px;
        border-radius: 8px;
        button {
            padding: 5px 10px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin: 0 5px;
        }
    }
</style>