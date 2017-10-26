<!--
  - Created by Mili on 2017/10/25
 -->

<template lang="html">
  <section class="container">
    <div class="div1">{{ testMsg }}</div>
    <div class="div2">{{ asyncMsg }}</div>
  </section>
</template>

<script>
  import axios from 'axios'
  export default {
    name: 'title',
    data () {
      return {
        testMsg: 'test.vue',
        asyncMsg: '我来自data'
      }
    },
    async asyncData (context) {
      let { data } = await axios.get('https://www.easy-mock.com/mock/59f1a18b54ea5676eb46308b/example/getUser')
      return {
        asyncMsg: data.data
      }
    }
  }
</script>
