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
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  gap: 200px;
}
</style>

<script setup>
import AppNavbar from '@/components/AppNavbar.vue'
import AppLogo from '@/components/AppLogo.vue'
</script>
