<script setup>
defineProps({
  height: {
    type: String,
  },
  width: {
    type: String,
  },
  borderRadius: {
    type: String,
  },
});
</script>
<template>
  <div class="dynamic-skeleton">&nbsp;</div>
</template>
<style scoped>
@keyframes bgAnimation {
  0% {
    background-position: 50% 0;
  }
  100% {
    background-position: -150% 0;
  }
}
.dynamic-skeleton {
  height: v-bind(height);
  width: v-bind(width);
  border-radius: v-bind(borderRadius);
  background-image: linear-gradient(
    to right,
    #d6d7d8 0%,
    #e2e3e4 10%,
    #d6d7d8 20%,
    #d6d7d8 100%
  );
  background-size: 200% 100%;
  /* box-shadow: 0 1px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1); */
  animation: bgAnimation 1.2s linear infinite;
  opacity: 0.6;
}
</style>
