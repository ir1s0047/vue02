<template>
  <div>
    回车：<input type="text" @keydown.enter="enterFn"><br>

    esc：<input type="text" @keydown.esc="escFn">
  </div>
</template>

<script>
export default {
  methods: {
    enterFn(){
      console.log('按下了回车');
    },
    escFn(){
      console.log('按下了esc');
    }
  }
}
</script>

<style>

</style>