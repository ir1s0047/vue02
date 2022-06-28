<template>
  <div>
    <p>你要购买的商品数量：{{count}} 件</p>
    <button v-on:click="count++">+1</button>
    <button @click="addFn">+2</button>
    <button @click="addCountFn(10)">+10</button>
    <button @click="js">-5</button>
    <button @click="clearFn">清空</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      count:0,
    }
  },
  methods:{
    addFn(){
      this.count+=2
    },
    addCountFn(val){
      this.count+=val
    },
    js(){
      this.count-=5
    },
    clearFn(){
      this.count=0
    }
  },

}
</script>

<style>

</style>