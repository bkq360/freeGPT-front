<script setup>
function test(){
    alert(111)
}

</script>
<template>
<div class="bottom userIcon"><img src="../../public/user.jpg" width="45px"></div>
<div class="bottom">Wender</div>
<div class="bottom">
    <button class="set-icon" @click="test">
      <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class=" iconify iconify--ri" width="22" height="22" viewBox="0 0 24 24"><path fill="currentColor" d="M2 12c0-.865.11-1.704.316-2.504A3 3 0 0 0 4.99 4.867a9.99 9.99 0 0 1 4.335-2.506a3 3 0 0 0 5.348 0a9.99 9.99 0 0 1 4.335 2.506a3 3 0 0 0 2.675 4.63c.206.8.316 1.638.316 2.503c0 .864-.11 1.703-.316 2.503a3 3 0 0 0-2.675 4.63a9.99 9.99 0 0 1-4.335 2.505a3 3 0 0 0-5.348 0a9.99 9.99 0 0 1-4.335-2.505a3 3 0 0 0-2.675-4.63C2.11 13.703 2 12.864 2 12m4.804 3c.63 1.091.81 2.346.564 3.524c.408.29.842.541 1.297.75A4.993 4.993 0 0 1 12 18c1.26 0 2.438.471 3.335 1.274c.455-.209.889-.46 1.297-.75A4.993 4.993 0 0 1 17.196 15a4.993 4.993 0 0 1 2.77-2.25a8.142 8.142 0 0 0 0-1.5A4.993 4.993 0 0 1 17.196 9a4.993 4.993 0 0 1-.564-3.524a7.991 7.991 0 0 0-1.297-.75A4.993 4.993 0 0 1 12 6a4.993 4.993 0 0 1-3.335-1.274a7.99 7.99 0 0 0-1.297.75A4.993 4.993 0 0 1 6.804 9a4.993 4.993 0 0 1-2.77 2.25a8.125 8.125 0 0 0 0 1.5A4.993 4.993 0 0 1 6.805 15M12 15a3 3 0 1 1 0-6a3 3 0 0 1 0 6m0-2a1 1 0 1 0 0-2a1 1 0 0 0 0 2"></path></svg>
    </button>
</div>
</template>
<style>
.bottom{
    margin: auto;
    overflow: hidden;
}
.userIcon{
    border-radius: 33px;
}
.set-icon{
    /* background-color: red; */
    width:35px;
    height:35px;
    border-radius: 33px;
    background-color: white;
    border: 0;
}
.set-icon:hover{
    background-color: rgba(233, 229, 229, 0.4);
    cursor: pointer;
}
</style>