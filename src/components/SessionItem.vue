<script setup>
import {ref,inject} from "vue";
const chooseIndex = inject("chooseIndex")
const isEdit = inject("isEdit")
const text = ref("New Chat");
const props = defineProps(['index'])
const itemIndex = props.index

// console.log(isEdit.value)
// const chooseIndex = props.chooseIndex
const emit = defineEmits(['changeSessionItemIndex','changeEditStatus'])

const changeSessions=(()=>{
    emit('changeSessionItemIndex',itemIndex)
    emit('changeEditStatus',false)
    // console.log(isEdit.value)
}) 
function alertSessionText(){
    // isEdit.value = true;
    emit('changeEditStatus',true)
    // console.log(isEdit.value)
}
function alertSessionSave(){
    emit('changeEditStatus',false)
}
function deleteSession(){
    alert("Are you comfirm delete this session?");
}
// changeSessions() 
</script>
<template>
 <div class="session-item" id="gogo" @mouseenter="showScrollbar" @mouseleave="hideScrollbar" @click="changeSessions"  > <!-- $emit('changeSession',index) -->
    <div class="item"> <svg  xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class="iconify iconify--ri front-img" width="1.1em" height="1.1em" viewBox="0 0 24 24"><path fill="currentColor" d="M2 8.994A5.99 5.99 0 0 1 8 3h8c3.313 0 6 2.695 6 5.994V21H8c-3.313 0-6-2.695-6-5.994zM20 19V8.994A4.004 4.004 0 0 0 16 5H8a3.99 3.99 0 0 0-4 3.994v6.012A4.004 4.004 0 0 0 8 19zm-6-8h2v2h-2zm-6 0h2v2H8z"></path></svg>
   </div>
    <div v-show="!isEdit|| itemIndex !== chooseIndex" class="item">  
        {{ text }}
    </div>
    <div v-show="!isEdit|| itemIndex !== chooseIndex" class="item">
        <div v-show="itemIndex == chooseIndex" class="item-alert-delete">
            <svg @click.stop="alertSessionText" xmlns="http://www.w3.org/2000/svg"  xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class=" iconify iconify--ri" width="1.1em" height="1.1em" viewBox="0 0 24 24"><path fill="currentColor" d="M6.414 15.89L16.556 5.748l-1.414-1.414L5 14.476v1.414zm.829 2H3v-4.243L14.435 2.212a1 1 0 0 1 1.414 0l2.829 2.829a1 1 0 0 1 0 1.414zM3 19.89h18v2H3z"></path></svg>
            &nbsp;
            <svg @click.stop="deleteSession" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class=" iconify iconify--ri" width="1.1em" height="1.1em" viewBox="0 0 24 24"><path fill="currentColor" d="M17 6h5v2h-2v13a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1V8H2V6h5V3a1 1 0 0 1 1-1h8a1 1 0 0 1 1 1zm1 2H6v12h12zm-9 3h2v6H9zm4 0h2v6h-2zM9 4v2h6V4z"></path></svg>
            </div>
    </div>
    <div class="item" v-show="isEdit && itemIndex == chooseIndex">
       <input class="input-text" type="text" :value="text" style="width:100%"/>
    </div>
    <div class="item" v-show="isEdit && itemIndex == chooseIndex">
        <svg @click.stop="alertSessionSave" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class=" iconify iconify--ri" width="1.1em" height="1.1em" viewBox="0 0 24 24"><path fill="currentColor" d="M7 19v-6h10v6h2V7.828L16.172 5H5v14zM4 3h13l4 4v13a1 1 0 0 1-1 1H4a1 1 0 0 1-1-1V4a1 1 0 0 1 1-1m5 12v4h6v-4z"></path></svg>
    </div>

    
 </div>
</template>
<style>
.front-img{
    pointer-events: none;
}

.session-item{
    display: grid;
    grid-template-columns: 0.5fr 1.8fr 0.7fr; /* 将容器分成三列，每列占用相同的空间 */
    font-size: small;
    align-items: center;
    height: 44px;
    line-height: 5px;
    margin:auto 15px 15px;
    padding-right: 5px; /* 滚动条的默认宽度（可以根据实际情况调整） */
    padding-left: 5px;
    border:1px solid rgba(192, 189, 189, 0.5);
    border-radius: 6px;
    text-align: center;
}
.item{
    display: flex;
    justify-content: center; /* 在主轴上居中 */
    align-items:center; /* 在交叉轴上居中 */
}
.item-alert-delete{
    display: flex;
    flex-direction: row;
    justify-content:flex-end;
    width: 80%;
}
.input-text{
    width:100%;
    border:1px  solid rgb(196, 193, 193,0.5);
    outline: none;
    /* border-color: rgb(80, 162, 99,1);  */
}
.input-text:hover{
    border-color: rgb(150, 205, 163);
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