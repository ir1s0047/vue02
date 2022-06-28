<template>
  <div>
    <span>{{sum()}}</span>
  </div>
</template>

<script>
export default {
    data () {
      return {
      
      }
    },
    methods: {
      sum(){
        let initialValue = 0
        let sum = [{a:100}, {a: 20}, {a:-10}].reduce((pre,cur)=>{
          return pre+cur.a
        },initialValue)
       console.log(sum);
      
      },

    }
}
</script>

<style>

</style>