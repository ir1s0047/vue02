<template>
  <div>
    <h1>{{msg}}</h1>
    <button @click="btn">翻转世界</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg:"你是年少的欢喜"
    }
  },
  methods: {
    btn(){
      // let arr = this.msg.split("")
      // // console.log(arr);
      // arr.reverse()
      this.msg = this.msg.split("").reverse().join("")
    }
  }
}
</script>

<style>

</style>