<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <link rel="stylesheet" href="/styles.css">

  <div>
    <header>
      <nav>
        <div class="navbar">
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
          <RouterLink to="/projects">Projects</RouterLink>
          <RouterLink to="/contact">Contact</RouterLink>
        </div>
      </nav>
    </header>

    <RouterView />
  </div>
</template>

<style scoped>

header {
  background-color: #041a30;
  color: #b8bfc4;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.2);
}

.navbar {
  display: flex;
  justify-content: space-around;
  padding: 10px;
}

nav a {
  color: #b8bfc4;
  text-decoration: none;
  transition: color 0.3s;
}

nav a:hover {
  color: #6e7e8d;
}

</style>