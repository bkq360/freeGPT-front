<script setup>
function autoResize() {
    const elementa = document.getElementById("inputsay");
    elementa.style.height = 'auto';
    elementa.style.height = (elementa.scrollHeight) + 'px';
}
function gogoa() {
    console.log("test")
}
function sendMs(){
    alert("send Message!");
}
</script>
<template>
    <div class="footer">
        <div class="foote-inner delete-icon">
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img"
                class="iconify iconify--ri" width="40" height="40" viewBox="-8 -8 40 40">
                <path fill="currentColor"
                    d="M17 6h5v2h-2v13a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1V8H2V6h5V3a1 1 0 0 1 1-1h8a1 1 0 0 1 1 1zm1 2H6v12h12zm-9 3h2v6H9zm4 0h2v6h-2zM9 4v2h6V4z">
                </path>
            </svg>
        </div>
        <div class="foote-inner history-icon">
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img"
                class=" iconify iconify--ri" width="40" height="40" viewBox="-8 -8 40 40">
                <path fill="currentColor"
                    d="M12 2c5.523 0 10 4.477 10 10s-4.477 10-10 10a9.956 9.956 0 0 1-4.708-1.175L2 22l1.176-5.29A9.956 9.956 0 0 1 2 12C2 6.477 6.477 2 12 2m0 2a8 8 0 0 0-8 8c0 1.335.326 2.618.94 3.766l.35.654l-.656 2.946l2.948-.654l.653.349A7.955 7.955 0 0 0 12 20a8 8 0 1 0 0-16m1 3v5h4v2h-6V7z">
                </path>
            </svg>
        </div>
        <div class="foote-inner select-icon">
            <div class="modelText">
                <span>模型：</span>
            </div>
            <select class="select-inner" name="test">
                <option value="3.5">默认GPT3.5</option>
                <option value="4">GPT4</option>
            </select>
        </div>
        <div class="foote-inner inputText">
            <textarea class="input-say" id="inputsay" @input="autoResize()" @focus="gogoa"
                placeholder="来说点什么吧...(Shift + Enter = 换行，&quot;/&quot; 触发提示词）"></textarea>
        </div>
        <div class="foote-inner bt-div">
            <button class="send-button n-bt" @click="sendMs" disabled>
                <div class="n-icon-slot">
                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                        role="img" class=" iconify iconify--ri" width="20" height="20" viewBox="0 0 24 24">
                        
                        <path fill="currentColor"
                            d="M1.946 9.315c-.522-.174-.527-.455.01-.634L21.044 2.32c.529-.176.832.12.684.638l-5.454 19.086c-.15.529-.455.547-.679.045L12 14l6-8l-8 6z">
                        </path>
                    </svg>
                </div>
            </button>
        </div>
    </div>
</template>
<style>
.footer {
    position: absolute;
    bottom: 20px;
    background-color: white;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    /* z-index: 1; */
}

.n-icon-slot {
    margin-top: 4px;
    margin-left: -3px;
}

.foote-inner {
    display: inline-block;
    text-align: center;
    margin-left: 15px;
}

.bt-div {
    height: 40px;
    width: 50px;
}

.inputText {
    width: 60%;
}

.n-bt {
    width: 48px;
    height: 35px;
    border-radius: 4px;
    color: white;
    /* background-color: #18a058; */
   
    background-color:  #96D0AF;
}

.input-say {
    width: 100%;
    height: auto;
    min-height: 35px;
    max-height: 160px;
    border: 1px solid rgba(192, 189, 189, 0.5);
    border-radius: 5px;
    resize: none;
}

.input-say:hover {
    border-color: rgb(80, 162, 99, 1);
}

.input-say:focus {
    border: 1px solid rgba(192, 189, 189, 0.5);

}

.select-icon {
    line-height: 40px;
    width: 160px;
}

.select-inner {
    height: 25px;
    width: 70%;
    vertical-align: center;
    max-width: 120px;
    border-color: rgba(106, 104, 104, 0.4);
    border-radius: 3px;
}

.modelText {
    display: inline-block;
}

.delete-icon,
.history-icon {
    width: 40px;
    border-radius: 20px;
    height: 40px;
}

.delete-icon:hover,
.history-icon:hover {
    background-color: rgba(224, 220, 220, 0.4);
    cursor: pointer;

}</style>
