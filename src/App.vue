<script setup>
import { ref, provide, reactive } from "vue";
import SpandButton from "./components/Button.vue";
import AddButton from "./components/AddButton.vue";
import SessionItem from "./components/SessionItem.vue";
import UserInfo from "./components/UserInfo.vue";
import SessionMain from "./components/SessionMain.vue";
import SessionFooter from "./components/SessionFooter.vue";

const isNoComponent = ref(true);
const sessionItemList = ref([]);
const chooseIndex = ref(0);
const isEdit = ref(true);
const ConversationList = reactive([])
provide("chooseIndex", chooseIndex);
provide("isEdit", isEdit);
provide("conversationList",ConversationList);
const spandDiv = () => {
  const element = document.getElementById("meun-right");
  const expandButton = document.getElementsByClassName("expand")[0];
  element.style.width = element.style.width === "0px" ? "14%" : "0px";
  expandButton.style.transform = `translateX(50%) translateY(-50%)${element.style.width === "0px" ? "" : " rotateY(180deg)"}`;
};

const showScrollbar = () => {
  document.getElementById("leftItemMain").style.overflow = "overlay";
};

const hideScrollbar = () => {
  document.getElementById("leftItemMain").style.overflow = "hidden";
};

const addSessionItem = () => {
  isNoComponent.value = false;
  sessionItemList.value.unshift(false);
  // ConversationList.value.unshift({"title":"","conversation":[]})
  insertObjectAtIndex(0,{"title":"","conversation":[]})
  // console.log(ConversationList[0])
  // console.log(ConversationList.value)
  changeIndex(0);
};
const insertObjectAtIndex=(index, object) => {
  ConversationList.splice(index, 0, object);
}
const changeIndex = (val) => {
  chooseIndex.value = val;
  sessionItemList.value = sessionItemList.value.map((_, index) => index === val);
};

const changeEditStatus = (bool) => {
  isEdit.value = bool;
};
</script>

<template>
  <div class="main">
    <div class="contain">
      <div class="main-right" id="meun-right">
        <div class="item-header">
          <AddButton @add-session-item="addSessionItem" />
        </div>
        <div class="item-main" id="leftItemMain" @mouseenter="showScrollbar" @mouseleave="hideScrollbar">
          <div class="default" v-if="isNoComponent">
            <div class="no-date-img">
              <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class="mb-2 text-3xl iconify iconify--ri" width="40" height="40" viewBox="0 0 30 30"><path fill="currentColor" d="M21 3a1 1 0 0 1 1 1v16a1 1 0 0 1-1 1H3a1 1 0 0 1-1-1V4a1 1 0 0 1 1-1zM7.416 14H4v5h16v-5h-3.416a5.001 5.001 0 0 1-9.168 0M20 5H4v7h5a3 3 0 1 0 6 0h5z"></path></svg>
            </div>
            <span>暂无数据</span>
          </div>
          <div v-else v-for="(sessionItem,index) in sessionItemList" :key="index">
            <SessionItem :class="{isChoose:sessionItem}" @changeEditStatus="changeEditStatus" @changeSessionItemIndex="changeIndex" :index="index" />
          </div>
        </div>
        <div class="item-bottom">
          <UserInfo />
        </div>
      </div>
      <SpandButton @click="spandDiv" />
      <div class="main-left">
        <SessionMain />
        <SessionFooter />
      </div>
    </div>
  </div>
</template>

<style>
body {
  margin: 0;
  padding: 0;
  height: 100vh;
  overflow: hidden;
}

html {
  overflow-y: auto;
  overflow-x: hidden;
}

.item-header {
  text-align: center;
  width: 100%;
  height: 100%;
}

.item-main {
  text-align: center;
  overflow: hidden;
  border-bottom: 1px solid rgb(196, 193, 193, 0.5);
}

.item-bottom {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  /* position:absolute; */
  bottom: 25px;
}

.default {
  display: grid;
  grid-template-columns: 1fr;
  color: rgb(225, 227, 228);
}

.no-date-img {
  width: 100%;
  height: 30px;
  text-align: center;
}

.main {
  width: 98%;
  box-shadow: 2px 3px 10px rgba(91, 91, 91, 0.3), -1px -1px 10px rgba(0, 0, 0, 0);
  border-radius: 6px;
  margin: auto;
  margin-top: 15px;
  min-height: calc(100vh - 30px);
  border: 1px solid rgb(196, 193, 193, 0.5);
  overflow: hidden;
}

.contain {
  display: flex;
}

.main-contain {
  position: relative;
  align-items: center;
}

.main-right {
  display: grid;
  grid-template-rows: 10% 80% 10%;
  position: relative;
  height: calc(100vh - 30px);
  width: 14%;
  border-right: 1px solid rgb(196, 193, 193, 0.4);
  transition: all ease 0.4s;
  overflow: hidden;
}

.main-left {
  position:relative;
  width: 100%;
  margin-left: -12px;
  /* display: grid; */
  /* grid-template-rows: 90% 10%; */
  height: calc(100vh - 30px);
}
</style>
