<script setup>
import {reactive,ref,computed,watch,onMounted} from 'vue'
import InputText from './InputText.vue';

const child = ref(null)

const count = ref(0)
const autocomputed = computed(()=>{
  return count.value+2
})
const obj = reactive({ count: 0 })
// instead, use a getter:
watch(
  () => obj.count,
  (count) => {
    console.log(`count is: ${count}`)
  }
)
defineProps({
  msg: String,
})
const arr = reactive([1,3,4,5,9]);
function test(){
  this.arr.push(16)
}
const test221 = ref(12)
function test22(){
  return test221;
}
//example ref 01:
const input = ref(null)
onMounted(()=>{
  input.value.focus()
  console.log(child.value.a)
})
//expample ref 02:
const list = ref([1,2])
const itemRefs  = ref([])
onMounted(()  =>  console.log(itemRefs.value))
//expample ref 03:
function inputtest(el){
  console.log(el)
}
</script>
<template>
  <!-- expample ref 02: -->
  <ul>
    <li v-for="item in list" :ref="itemRefs">
      {{ item }}
    </li>
  </ul>
   <!-- expample ref 01: -->
 <input ref="input">
  <!-- expample ref 03: -->
  <ul>
    <li v-for="item in list" :ref="inputtest">
      {{ item }}
    </li>
  </ul>

  <div class="card">
    <button type="button" @click="obj.count++">count is {{ obj.count }}</button>
    <button type="button" :prop="data" @click="test()">count</button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  
  {{ autocomputed }}
  <InputText  @event="test22" class="active" ref="child"/>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
