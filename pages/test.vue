<!--
  - Created by Mili on 2017/10/25
 -->

<template lang="html">
  <section class="container">
    <div class="div1">{{ testMsg }}</div>
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
