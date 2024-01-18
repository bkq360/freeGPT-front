<script setup>
import {ref,inject} from "vue";
const list = inject("sessionList")
const text = ref("New Chat");
function changeSession(event){
    const sessionItem = event.target;
    const index = sessionItem.getAttribute("index");
    for(let i =0;i<list.value.length;i++){
        if(i == index){
            list.value[i] = true
        }else{
            list.value[i] = false;
        }
    }
}
</script>
<template>
 <div class="session-item" id="gogo" @mouseenter="showScrollbar" @mouseleave="hideScrollbar" @click="changeSession">
    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="M2 8.994A5.99 5.99 0 0 1 8 3h8c3.313 0 6 2.695 6 5.994V21H8c-3.313 0-6-2.695-6-5.994zM20 19V8.994A4.004 4.004 0 0 0 16 5H8a3.99 3.99 0 0 0-4 3.994v6.012A4.004 4.004 0 0 0 8 19zm-6-8h2v2h-2zm-6 0h2v2H8z"></path></svg>
   {{ text }}
   <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="M6.414 15.89L16.556 5.748l-1.414-1.414L5 14.476v1.414zm.829 2H3v-4.243L14.435 2.212a1 1 0 0 1 1.414 0l2.829 2.829a1 1 0 0 1 0 1.414zM3 19.89h18v2H3z"></path></svg>
   <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24"><path fill="currentColor" d="M17 6h5v2h-2v13a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1V8H2V6h5V3a1 1 0 0 1 1-1h8a1 1 0 0 1 1 1zm1 2H6v12h12zm-9 3h2v6H9zm4 0h2v6h-2zM9 4v2h6V4z"></path></svg>
 </div>
</template>
<style>
.session-item{
    height: 46px;
    line-height: 46px;
    margin:auto 15px 15px;
    padding-right: 17px; /* 滚动条的默认宽度（可以根据实际情况调整） */
    border:1px solid rgb(196, 193, 193,0.5);
    border-radius: 6px;
    text-align: center;
}
.isChoose{
    border-color: rgb(80, 162, 99,1);
    color:rgb(80, 162, 99,1);
}
.session-item:hover{
    background-color: rgb(246, 243, 243);
    cursor: pointer;
}
</style>