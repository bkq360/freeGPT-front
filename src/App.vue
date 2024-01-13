<script setup>
</script>
<template>
  <div class="main" > 
    <div class="contain">
      <div class="tab">
        
      </div>
      <div class="content">
        
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
  box-shadow:2px 3px 2px rgba(0, 0, 0, 0.3);
  margin:auto;
  margin-top:15px;
  min-height:calc(100vh - 30px);
  border:1px solid rgb(196, 193, 193)
}
.contain{
  display: flex;
}
.tab{
  height:calc(100vh - 30px);
  width:14%;
}
.content{
  height:calc(100vh - 30px);
  width:86%;
}
</style>
