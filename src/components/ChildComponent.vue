<template>
    <div>
      <p>Is Activated: {{ isActivated }}</p>
      <button @click="toggleActivation">Toggle Activation</button>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      isActivated: Boolean
    },
    methods: {
      toggleActivation() {
        this.$emit('update:isActivated', !this.isActivated);
      }
    }
  };
  </script>