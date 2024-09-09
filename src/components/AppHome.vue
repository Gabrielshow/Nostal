<template>
  <div class="scroll-text">
    <span> This is a scolling text</span>
  </div>
</template>
<style scoped>
.scroll-text {
  position: relative;
  width: 100%;
  overflow: hidden;
}
.scroll-text span {
  text-align: center;
  position: absolute;
  white-space: nowrap;
  animation: scroll 10s linear infinite;
}

@keyframes scroll {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(-100%);
  }
}
</style>
<script setup></script>
