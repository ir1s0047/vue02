<template>
  <div>
    <a @click="one" href="http://www.baidu.com">去百度</a> <br>
    <a @click="two(1,$event)" href="http://www.baidu.com">阻止去百度事件</a>
  </div>
</template>

<script>
export default {
  data () {
    return {
      
    }
  },
  methods: {
    one(e){
      e.preventDefault();
    },
    two(num,e){
      e.preventDefault();
    }
  }
}
</script>

<style>

</style>