<template>
  
  <div class="app">

    <Sidebar />

    <!-- it is the router view  -->
    <router-view />

  </div>

</template>

<script setup>

import Sidebar from './components/Sidebar.vue'

</script>

<style lang="scss">
:root {
  --primary: #4ade80;
  --grey: #64748b;
  --dark: #1e293b;
  --dark-alt: #334155;
  --light: #f1f5f9;
  --sidebar-width: 300px;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: 'Fire Sans', sans-serif;
}

body {
  background: var(--light);
}

button {
  cursor: pointer;
  appearance: none;
  border: none;
  background: none;
  outline: none;
}

.app {
  display: flex;
  
  main { 
    flex: 1 1 0;
    padding: 2rem;

    @media (max-width: 768px) {
      padding-left: 6rem;
      
    }
  }
}
</style>
