<template>
<div>
  <div v-for="(item,index) in dataList" :key="index">
    <h5 @click="movePage(index)">{{item.title}}</h5>
    <p>{{item.date}}</p>
  </div>
</div>
</template>

<script>
export default {
    name : 'List',
    props:{
        dataList:Array,
    },
    methods: {
      movePage(idx){
          this.$router.push(`/detail/${idx}`) //route,router 차이
      }  
    },
}
</script>

<style>

</style>