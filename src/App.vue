<template>
  <div id="app">
{{obj}}
    <button @click="cl"></button>
  </div>
</template>
<script>
  export default {
    data(){
     return{
       obj:{
         name:'zxx',
         age:20
       }
     }
    }
    ,methods:{
      cl(){
        this.$set(this.obj,"name",111111)
        this.$delete(this.obj,"name")
      }
    }
  }
</script>

<style lang="less">


</style>
