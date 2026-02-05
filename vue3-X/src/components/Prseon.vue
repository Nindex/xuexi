
<template>
  <div class="perseon">
    <h1>姓名：{{ name }}</h1>
    <p>年龄：{{ age }}</p>

  </div>
</template>

<script lang="ts">

export default {
  name: 'Perseon',
  setup() {
    // 数据
      let name: '张三'
      let age: 18
      let TEL: '13800000000'
    return {name,age,TEL}
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