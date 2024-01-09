<script setup>
defineProps({
    title: String,
    likes: Number
  })
// let width = (document.documentElement.clientWidth-700)+"px";
// let height = (document.documentElement.clientHeight-100)+"px";
</script>

<template>
  test
  <div class="main" :style="{width:width,height:height}" > 
    test
  </div>
</template>
<style >
body,*{
  margin:0;
  padding:0;
}
.main{
  width:100%; 
   height:100%;
  background-color:red;
  /* padding:0px; */
  /* margin:50px; */
}

</style>
