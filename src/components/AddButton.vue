<script setup>
</script>
<template>
        <button class="add-button" @click="$emit('addSessionItem')">新建聊天</button>
</template>
<style>
.add-button{
    width: 88%;
    height: 32px;
    margin-top: 7%;
    cursor:pointer;
    font-weight: 350;
    background: rgba(255, 255, 255, 1);
    border:1px dashed rgb(196, 193, 193,0.5);
    border-radius: 6px;
    z-index: 0;
}
.add-button:hover{
    border-color: rgb(80, 162, 99,1);
    color:rgb(80, 162, 99,1);
}

</style>