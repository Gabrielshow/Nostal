<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <nav class="routes">
    <RouterLink to="/about"> <li>About</li> </RouterLink>
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
}
.routes a {
  text-decoration: none;
  color: black;
}

.routes a:hover {
  background: linear-gradient(to right, #424, #398);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  scale: 1.1;
}
.routes li {
  list-style-type: none;
}
</style>
