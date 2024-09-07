<script setup></script>

<template>
  <nav class="routes">
    <li>About</li>
    <li>Contact</li>
    <li>Order</li>
  </nav>
</template>

<style>
.routes {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
  gap: 20px;
}
.routes li {
  list-style-type: none;
}
</style>
