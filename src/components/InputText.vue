<script setup>
import {reactive,ref,computed} from 'vue'
const isactive=ref(false)
const isdanger  = ref(true)
const a = 1
const b = ref(2)

// Compiler macros, such as defineExpose, don't need to be imported
defineExpose({
  a,
  b
})
</script>
<style scoped>
.active{
    color: red;
    background-color:red;
    width:500px;
    height:600px;
}
.danger{
    width:900px;
    height:600px;
    color:rebeccapurple;
    background-color:yellowgreen;
}
</style>
<template>
    <el-input @v-model="$emit('test22')" placeholder="Please input" />
    <div :class="$attrs.class" class="danger" with="500" height="500"></div>
</template>
  
  <!-- <script lang="ts" setup>
  import { ref } from 'vue'
  </script> -->