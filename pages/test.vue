<!--
  - Created by Mili on 2017/10/25
 -->

<template lang="html">
  <section class="container">
    <div>{{ testMsg }}</div>
  </section>
</template>

<script>
  export default {
    name: 'title',
    data () {
      return {
        testMsg: '我是测试的数据'
      }
    }
  }
</script>

<style>
  .container {
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }
</style>
