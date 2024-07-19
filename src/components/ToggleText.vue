<template>
    <div>
      <button class="toggle-button" @click="toggleText">{{ isVisible ? '-' : '+' }}</button>
      <p v-if="isVisible" class="toggle-text">This is the additional text that can be shown or hidden.</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isVisible: false
      };
    },
    methods: {
      toggleText() {
        this.isVisible = !this.isVisible;
      }
    }
  };
  </script>
  
  <style scoped>
  .toggle-button {
    font-size: 1.5rem;
    cursor: pointer;
  }
  .toggle-text {
    margin-top: 10px;
    font-size: 1rem;
  }
  </style>
  