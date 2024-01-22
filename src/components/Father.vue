<template>
    <div>
      <ChildComponent :isActivated.sync="isActivated" />
      <ChildComponent :isActivated.sync="!isActivated" />
    </div>
  </template>
  
  <script>
  import ChildComponent from './ChildComponent.vue';
  
  export default {
    components: {
      ChildComponent
    },
    data() {
      return {
        isActivated: false
      };
    }
  };
  </script>