<template>
  <div>
    <button @click="jump()">点击一下</button>
  </div>
</template>

<script>
export default {
  name: 'InnerPage',
  data () {
    return {
      msg: 'hello inner'
    }
  },

  //  方法
  methods: {
    jump () {
      console.log('测试')
      this.$router.push({path: '/'})
    }
  }

}
</script>

<style scoped>

</style>
