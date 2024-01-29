<script setup>
import { ref,provide } from "vue";
import SpandButton from "./components/Button.vue"
import AddButton from "./components/AddButton.vue"
import SessionItem from "./components/SessionItem.vue"
import UserInfo from "./components/UserInfo.vue"
import SessionMain from "./components/SessionMain.vue"
// export default defineComponent({
//   // 需要启用子组件作为模板
//   components: {
//     Child,
//   },

//   // 定义一些数据并 `return` 给 `<template />` 用
//   setup() {
//     const userInfo: Member = {
//       id: 1,
//       name: 'Petter',
//     }

//     // 不要忘记 `return` ，否则 `<template />` 拿不到数据
//     return {
//       userInfo,
//     }
//   },
// })

const isNoComponent = ref(true)
const sessionItemList = ref([])
const chooseIndex = ref(0)
const isEdit = ref(true);
provide("chooseIndex",chooseIndex)
provide("isEdit",isEdit)
function spandDiv(){
  let element = document.getElementById("meun-right");
  let expandButton = document.getElementsByClassName("expand")[0];
  if(element.style.width == "0px"){
    element.style.width = "14%";
    expandButton.style.transform = "translateX(50%) translateY(-50%) rotateY(180deg)";
  }else{
    element.style.width = "0px";
    expandButton.style.transform = "translateX(50%) translateY(-50%)";
  }
}
function showScrollbar(){
    document.getElementById("leftItemMain").style.overflow = 'overlay';
}
function hideScrollbar() {
     document.getElementById("leftItemMain").style.overflow = 'hidden';
}
function addSessionItem(){
  if(isNoComponent.value){
    isNoComponent.value = false;
  }
  sessionItemList.value.unshift(false);
  changeIndex(0)
}

function changeIndex(val){
  for(let i =0;i<sessionItemList.value.length;i++){
        if(i == val){
          chooseIndex.value = i
          // console.log(chooseIndex.value)
          sessionItemList.value[i] = true    
        }else{
          sessionItemList.value[i] = false;
        }
    }  
    // changeEditStatus()
    // isEdit.value= false; 
}
function changeEditStatus(bool){
  // alert("in")
  isEdit.value = bool;
}
</script>
<template>
  <div class="main" > 
    <div class="contain">
      <div class="main-content"></div>
      <div class="main-right" id="meun-right" >
        <div class="item-header">
          <AddButton @add-session-item="addSessionItem"/>
        </div>
        <div class="item-main" id="leftItemMain"  @mouseenter="showScrollbar" @mouseleave="hideScrollbar">
         <div class="default" v-if="isNoComponent">
              <div class="no-date-img">
                <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class="mb-2 text-3xl iconify iconify--ri" width="40" height="40" viewBox="0 0 30 30"><path fill="currentColor" d="M21 3a1 1 0 0 1 1 1v16a1 1 0 0 1-1 1H3a1 1 0 0 1-1-1V4a1 1 0 0 1 1-1zM7.416 14H4v5h16v-5h-3.416a5.001 5.001 0 0 1-9.168 0M20 5H4v7h5a3 3 0 1 0 6 0h5z"></path></svg>
              </div>
              <span>暂无数据</span>
         </div>
         <div v-else v-for="(sessionItem,index) in sessionItemList" :key="index">
              <SessionItem   :class="{isChoose:sessionItem}" @changeEditStatus="changeEditStatus" @changeSessionItemIndex="changeIndex" :index="index"  />
            </div>
        </div>
        <div class="item-bottom">
          <UserInfo/>
        </div>
      </div>
      <SpandButton @click="spandDiv"/>
      <div class="main-left">
        <SessionMain />
      </div>
    </div>
  </div>
</template>
<style >
body{
  margin:0;
  padding:0;
  height:100vh;
  overflow: hidden; 
}
html {
    overflow-y: auto;
    overflow-x: hidden;
  }
.item-header{
  text-align: center;
  width:100%;
  height: 100%;
}
.item-main{
  text-align: center;
  overflow: hidden;
  border-bottom: 1px solid rgb(196, 193, 193,0.5);
}
.item-bottom{
  /* text-align: center; */
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;

}
.default{
  display: grid;
  grid-template-columns: 1fr;
  color: rgb(225, 227, 228);

}
.no-date-img{
  width:100%;
  height: 30px;
  text-align: center;
}
.main{
  width:98%;
  box-shadow:2px 3px 10px rgba(91, 91, 91, 0.3),-1px -1px 10px rgba(0,0,0,0);
  border-radius: 6px;
  margin:auto;
  margin-top:15px;
  min-height:calc(100vh - 30px);
  border:1px solid rgb(196, 193, 193,0.5);
  overflow: hidden;
}
.contain{
  display: flex;
}
.main-contain{
  position: relative;
  align-items:center
}
.main-right{
  display: grid;
  grid-template-rows: 10% 80% 10%;
  position:relative;
  height:calc(100vh - 30px);
  width:14%;
  border-right:1px solid rgb(196, 193, 193,0.4);
  transition: all ease 0.4s;
  overflow: hidden;
}
.main-left{
  height:calc(100vh - 30px); 
}
</style>
