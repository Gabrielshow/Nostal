<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <nav class="routes">
    <router-link to="/about"> <li>About</li> </router-link>
    <RouterLink to="/contact"><li>Contact</li></RouterLink>
    <RouterLink to="Book"><li>Order</li> </RouterLink>
  </nav>
</template>

<style>
.routes {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
  gap: 40px;
  padding: 0 4px;
  font-family: Didot;
}
.routes a {
  text-decoration: none;
  color: white;
}

.routes a:hover {
  background: linear-gradient(to right, #424, #398);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  scale: 1.1;
}
.routes a:active {
  background: linear-gradient(to right, #424, #398);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.routes li {
  list-style-type: none;
}
</style>
