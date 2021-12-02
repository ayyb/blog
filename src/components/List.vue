<template>
<div>
  <div v-for="(item,index) in dataList" :key="index">
    <h5>{{item.title}}</h5>
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
}
</script>

<style>

</style>