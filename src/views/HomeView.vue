<!-- App.vue -->
<template>
  <div class="app">
    <nav-bar></nav-bar>
    <menu-item />

    <!-- Barre de recherche -->
    <div class="search-container">
      <input type="text" placeholder="Search" class="search-bar">
    </div>
  </div>
</template>

<script>
import MenuItem from '../components/content/MenuItem.vue'
import NavBar from '../components/headers/NavBar.vue'
export default {
  components: { NavBar, MenuItem },
  name: 'App',
}
</script>

<style scoped>
.app {
  min-height: 100vh;
  background: linear-gradient(45deg, #1a1a2e 0%, #4a1259 50%, #c70039 100%);
  padding: 0rem;
}

.search-container {
  position: fixed;
  bottom: 2rem;
  left: 50%;
  transform: translateX(-50%);
  width: 90%;
  max-width: 600px;
}

.search-bar {
  width: 100%;
  padding: 1rem 2rem;
  border-radius: 30px;
  border: none;
  background: rgba(255, 255, 255, 0.9);
  backdrop-filter: blur(5px);
  font-size: 1rem;
}

.search-bar:focus {
  outline: none;
  background: white;
}


</style>