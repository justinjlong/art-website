<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <nav class="mt-0">
        <h3 class="mx-3">Justin J. Long - Art.</h3>
        <!-- <hr width="95%" class="mx-1"> -->
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
        <RouterLink to="/recentWork">Recent Work</RouterLink>
      </nav>
    </div>
    
  </header>

  <RouterView />

</template>

<style scoped>
header {
  line-height: 1.5;
  
}

.wrapper {
  background-color: #fafafa;
  padding: 0 1rem;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    place-items: center;
  }

  nav {
    text-align: left;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
