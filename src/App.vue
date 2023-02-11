<template>
  <v-app>
    <v-main>
       <header >
          <div class="wrapper pl-8">
            <nav>
              <RouterLink to="/">Home</RouterLink>
              <RouterLink to="/about">About</RouterLink>
              <RouterLink to="/recentWork">RecentWork</RouterLink>
              <RouterLink to="/1">Contact</RouterLink>
              <RouterLink to="/2">Store</RouterLink>
            </nav>
          </div>
        </header>
        <div class="pa-8">
          <RouterView />
        </div>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { RouterLink, RouterView } from 'vue-router'

export default defineComponent({
  name: 'App',

  data () {
    return {
      RouterLink,
      RouterView
    }
  },
})
</script>
<style scoped>
.body,
.v-application{
    font-family: 'Times New Roman';
}

header {
  line-height: 1.5;
  max-height: 100vh;
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
nav a {
  color: #9fc7b0;
  text-decoration:none;
}
nav a.router-link-exact-active {
  color: #2c3e50;
}
nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid black;
}
nav a:first-of-type {
  border: 0;
}
@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
  .logo {
    margin: 0 2rem 0 0;
  }
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>