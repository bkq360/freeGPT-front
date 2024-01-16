<script setup>
import { onMounted } from "vue";
import Button from "./components/button.vue"
onMounted(()=>{
  // function test(){
  //   alert(111)
  // }
})
function test(){
  let element = document.getElementById("meun-right");
  let expandButton = document.getElementsByClassName("expand")[0];
  let width = window.getComputedStyle(element).width;
  if(element.style.width == "0px"){
    element.style.width = "14%";
    expandButton.style.transform = "translateX(50%) translateY(-50%) rotateY(180deg)";
  }else{
    element.style.width = "0px";
    expandButton.style.transform = "translateX(50%) translateY(-50%)";
  }

  // element.button.style.transform="rotateY(180deg)";
  // element.style.width = width != "0px" ? "0px" : "14%";
  
}
</script>
<template>
  <div class="main" > 
    <div class="contain">
      <div class="main-content"></div>
      <div class="main-right" id="meun-right" >
        test
      </div>
      <Button @click="test" />
      <div class="main-left">
        testa
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

.main{
  width:98%;
  box-shadow:2px 3px 2px rgba(0, 0, 0, 0.3),-1px -1px 1px rgba(0,0,0,0.05);
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
  position:relative;
  height:calc(100vh - 30px);
  width:14%;
  /* left:0; */
  border-right:1px solid rgb(196, 193, 193,0.5);
  /* width:0px; */
  
  transition: all ease 0.4s;
  overflow: hidden;
}
.main-left{
  height:calc(100vh - 30px);
  
}
</style>
