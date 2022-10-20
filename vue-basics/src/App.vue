<script setup>

</script>

<template>
  <header>
 
    <div class="app">
      <div class="nav">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </div>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>

  .app {
    margin-bottom: 1rem;
    padding-left: 1rem;
    padding-right: 1rem;
  }
  .nav {
    display: flex;
    align-content: center;
    justify-content: space-between;
    padding: 1rem;
    width: 30rem;
  }

</style>
