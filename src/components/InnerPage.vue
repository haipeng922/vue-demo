<template>
  <div>
    <button @click="jump()">点击一下</button>
    <van-button type="primary">主要按钮</van-button>
    <van-button type="info">信息按钮</van-button>
    <van-button type="default">默认按钮</van-button>
    <van-button type="warning">警告按钮</van-button>
    <van-button type="danger">危险按钮</van-button>
  </div>
</template>

<script>
import { Button } from 'vant'
export default {
  components: {
    [Button.name]: Button
  },
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
