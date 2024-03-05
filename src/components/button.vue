<script setup>
 
</script>
<template>
    <div class="expand" >
        <i>
        <svg viewBox="0 0 16 16" fill="none" opacity="0.6"><path d="M5.64645 3.14645C5.45118 3.34171 5.45118 3.65829 5.64645 3.85355L9.79289 8L5.64645 12.1464C5.45118 12.3417 5.45118 12.6583 5.64645 12.8536C5.84171 13.0488 6.15829 13.0488 6.35355 12.8536L10.8536 8.35355C11.0488 8.15829 11.0488 7.84171 10.8536 7.64645L6.35355 3.14645C6.15829 2.95118 5.84171 2.95118 5.64645 3.14645Z" fill="currentColor"></path></svg>
        </i>
    </div>
</template>
<style>
i{
    font-style: italic;
}
.expand{
    border-radius: 50%;
    border:1px  solid rgb(196, 193, 193,0.5) ;
    position:relative;
    margin: auto 0;
    left: -24px;
    width: 24px;
    height:21px;
    cursor: pointer;
    background-color:#FFF;
    transform:translateX(50%) translateY(-50%) rotateY(180deg);
    /* z-index:1; */
    box-shadow: 0 2px 4px 0px rgba(0,0,0,.06);
    
    /* transform: rotateY(180deg); */
    
}
</style>