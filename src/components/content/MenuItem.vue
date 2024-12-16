<template>
    <div>
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
    </div>
</template>

<script setup>

</script>

<style  scoped>
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
</style>