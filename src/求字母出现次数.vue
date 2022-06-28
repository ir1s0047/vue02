<template>
  <div>
    {{num()}}
  </div>
</template>

<script>
export default {
  methods: {
    num(){
      let str = 'asdxcssasaaxd';
      let names = str.split('');

      let countedNames = names.reduce(function (allNames, name) {
        if (name in allNames) {
          allNames[name]++;
        } else {
          allNames[name] = 1;
        }
        return allNames;
      }, {});
      console.log(countedNames);
    }
  }
}
</script>

<style>

</style>