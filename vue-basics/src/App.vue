<template>
  <header class="header">
 
    <div class="app">
      <div class="nav">
        <RouterLink class="router home" to="/">Home</RouterLink>
        <header>|</header>
        <RouterLink class="router about" to="/about">About</RouterLink>
        <header>|</header>
        <RouterLink class="router yes" to="/yes">...</RouterLink>
      </div>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>

  .header {
    background-color: #3b2e4a;
  }
  .app {
    margin-bottom: 1rem;
    padding-left: 1rem;
    padding-right: 1rem;
  }  
  
  a {
    text-decoration: none;
    color: inherit;
  }
  .nav {
    display: flex;
    align-content: center;
    padding: 2rem;
    margin: 0rem;
    font-size: 2rem;
    color:#c9c9c9
  }

  .router + header {
    margin-left: 5rem;
  }

  header + .router {
    margin-left: 5rem;
  }

  .router:hover {
    text-decoration: underline;
  }

  .router:active {
    color: #407de4;
  }

</style>
