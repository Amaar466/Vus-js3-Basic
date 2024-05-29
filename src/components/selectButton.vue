<template>
    <div id="app">
      <button v-for="(button, index) in buttons" :key="index"
              :class="{'selected': selectedIndices.includes(index), 'custom-button': button.custom}"
              @click="selectButton(index)">
        {{ button.label }}
      </button>
    </div> 
  
    <div class="row">
        <input type="text">
        <input type="text">
        <input type="text" size="15">
        <input type="text" size="8">
    </div>

  </template>
  
  <script>
  export default {
    data() {
      return {
        buttons: [
          { label: 'new 1', custom: true },
          { label: 'new 2', custom: false },
          { label: 'new 3', custom: false },
          { label: 'new 4', custom: false },
          { label: 'new 5', custom: false }
        ],
        selectedIndices: []
      };
    },
    methods: {
      selectButton(index) {
        const selectedIndex = this.selectedIndices.indexOf(index);
        if (selectedIndex > -1) {
          // If the button is already selected, remove it from the selected indices
          this.selectedIndices.splice(selectedIndex, 1);
        } else {
          // Otherwise, add it to the selected indices
          this.selectedIndices.push(index);
        }
      }
    }
  };
  </script>
  
  <style scoped>
  .selected {
    background-color: yellow;
  }
  
  .custom-button {
    /* Additional styles for custom button */
  }
  
  button:hover {
    background-color: lightgray;
  }
  </style>
  