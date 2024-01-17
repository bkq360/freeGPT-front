<script setup>
import { onMounted } from "vue";
import Button from "./components/Button.vue"
import AddButton from "./components/AddButton.vue"
function test(){
  let element = document.getElementById("meun-right");
  let expandButton = document.getElementsByClassName("expand")[0];
  if(element.style.width == "0px"){
    element.style.width = "14%";
    expandButton.style.transform = "translateX(50%) translateY(-50%) rotateY(180deg)";
  }else{
    element.style.width = "0px";
    expandButton.style.transform = "translateX(50%) translateY(-50%)";
  }
  
 
  function showScrollbar() {
    alert("in")
      document.getElementById("leftItemMain").style.overflow = 'auto';
  }
  function hideScrollbar() {
    document.getElementById("leftItemMain").style.overflow = 'hidden';
  }
  function testgo(){
    alert(1111)
  }


}
</script>
<template>
  <div class="main" > 
    <div class="contain">
      <div class="main-content"></div>
      <div class="main-right" id="meun-right" >
        <div class="item-header">
          <AddButton />
        </div>
        <div class="item-main"    @mouseenter="showScrollbar"
      @mouseleave="hideScrollbar">
          <SessionItem />
          <SessionItem />
          <SessionItem />
          <SessionItem />
          <SessionItem />
          <SessionItem />
          <SessionItem />
          <SessionItem />
          <SessionItem />
          <SessionItem />
          <SessionItem />
          <SessionItem />
        </div>
        <div class="item">3</div>
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
.item-header{
  text-align: center;
  width:100%;
  height: 100%;
}
.item-main{
  text-align: center;
  overflow: hidden;
}
.scroll::-webkit-scrollbar{
display: none;
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
  grid-template-rows: 10% 65% 25%;
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
