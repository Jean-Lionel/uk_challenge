<template>
    <div>
        <!-- Barre de navigation -->
        <nav class="nav">
            <div class="nav-items">
                <div class="logo">
                    <img src="../../assets/img/logo.png" alt="">
                </div>
                <span>Profile</span>
                <span>Settings</span>
                <span>Billing</span>
                <span>Help</span>
            </div>
        </nav>
        
    </div>
</template>

<script setup>

</script>

<style  scoped>
.logo img{
    width: 30px;
}
.nav {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    color: black;
    padding: 1rem;
    background: #fff;
  }
  
  .nav-items {
    display: flex;
    gap: 2rem;
  }
  
  .nav-items span {
    cursor: pointer;
  }

</style>