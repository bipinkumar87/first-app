<template>
    <div class="app-container">
      <div class="typing-container">
        <p>{{ displayedText }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
      name:'AniMate',
    data() {
      return {
        fullText: 'Hello, welcome to the typing animation demo!',
        displayedText: '',
        typingIndex: 0,
        typingSpeed: 100 // typing speed in milliseconds
      };
    },
    mounted() {
      this.startTypingAnimation();
    },
    methods: {
      startTypingAnimation() {
        this.typingInterval = setInterval(() => {
          if (this.typingIndex < this.fullText.length) {
            this.displayedText += this.fullText[this.typingIndex];
            this.typingIndex++;
          } else {
            clearInterval(this.typingInterval);
          }
        }, this.typingSpeed);
      }
    },
    beforeUnmount() {
      clearInterval(this.typingInterval);
    }
  };
  </script>
  
  <style>
  .app-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #f5f5f5;
    font-family: Arial, sans-serif;
  }
  
  .typing-container {
    padding: 20px;
    border: 2px solid #ccc;
    border-radius: 10px;
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  .typing-container p {
    font-size: 24px;
    white-space: pre-wrap; /* Preserve whitespace */
    overflow-wrap: break-word;
  }
  </style>
  