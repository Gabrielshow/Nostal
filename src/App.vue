<template>
  <div class="main">
    <AppLogo />
    <AppNavbar />
  </div>
</template>

<style scoped>
.main {
  margin: 0px;
  padding: 0px 4px;
  width: 100vw;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  /* background: linear-gradient(to right, #424, #398); */
  height: 100px;
  border-left: 5px solid orange;
}
</style>

<script setup>
import AppNavbar from '@/components/AppNavbar.vue'
import AppLogo from '@/components/AppLogo.vue'
</script>
