<!-- App.vue -->
<template>
  <div class="app">
    <!-- Barre de navigation -->
    <nav class="nav">
      <div class="logo">☘️</div>
      <div class="nav-items">
        <span>Profile</span>
        <span>Settings</span>
        <span>Billing</span>
        <span>Help</span>
      </div>
    </nav>

    <!-- Grille d'icônes -->
    <div class="icon-grid">
      <div class="icon-box">
        <div class="icon chat-icon">💬</div>
      </div>
      <div class="icon-box">
        <div class="icon heart-icon">❤️</div>
      </div>
      <div class="icon-box">
        <div class="icon telegram-icon">✈️</div>
      </div>
      <div class="icon-box">
        <div class="icon play-icon">▶️</div>
      </div>
      <div class="icon-box">
        <div class="icon location-icon">📍</div>
      </div>
      <div class="icon-box">
        <div class="icon grid-icon">⊞</div>
      </div>
    </div>

    <!-- Barre de recherche -->
    <div class="search-container">
      <input type="text" placeholder="Search" class="search-bar">
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>

<style scoped>
.app {
  min-height: 100vh;
  background: linear-gradient(45deg, #1a1a2e 0%, #4a1259 50%, #c70039 100%);
  padding: 1rem;
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
  padding: 1rem;
}

.nav-items {
  display: flex;
  gap: 2rem;
}

.nav-items span {
  cursor: pointer;
}

.icon-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1rem;
  max-width: 300px;
  margin: 2rem 0;
}

.icon-box {
  background: rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 1rem;
  backdrop-filter: blur(5px);
  cursor: pointer;
  transition: transform 0.2s;
}

.icon-box:hover {
  transform: scale(1.05);
}

.icon {
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 24px;
  background: white;
  border-radius: 12px;
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