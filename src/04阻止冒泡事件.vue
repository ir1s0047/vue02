<template>
  <div @click="fatherFn">
    <button @click.stop="btn">.stop 阻止事件冒泡</button><br>
    <a href="http://www.baidu.com" @click.prevent="btn">.prevent阻止默认事件行为</a><br>
    <button @click.once="btn">.once程序运行期间, 只触发一次事件处理函数</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      
    }
  },
  methods: {
    fatherFn(){
      console.log('fatherFn被触发');
    },
    btn(){
      console.log(1);
    }
  }
}
</script>

<style>

</style>