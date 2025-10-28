
<template>
  <div id="app">
    <header>
      <h1>Tindung Vue App</h1>
      <nav>
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link>
      </nav>
    </header>
    <main>
      <router-view />
    </main>
  </div>
</template>

<script setup>
// No imports needed for router-view or router-link
</script>

<style>
body { font-family: system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; margin: 0; padding: 1rem; }
#app { max-width: 800px; margin: 0 auto; }
header h1 { color: #42b883; }
nav { margin-bottom: 1rem; }
nav a { color: #42b883; text-decoration: none; margin: 0 0.5rem; }
nav a.router-link-exact-active { font-weight: bold; }
</style>
