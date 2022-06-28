<template>
  <div>
    <h1>{{msg}}</h1>
    <h2>{{obj.author}}</h2>
    <h3>{{obj.class}}</h3>
    <h3>{{obj.time>=120?"长片":"短片"}}</h3>
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg:"奇异博士2",
      obj:{
        author:"漫威影业",
        class:"恐怖片",
        time:"130"
      }
    }
  }
}
</script>

<style>

</style>