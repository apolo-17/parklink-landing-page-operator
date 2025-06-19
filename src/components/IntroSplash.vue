<template>
  <div
    class="fixed inset-0 z-50 flex items-center justify-center bg-white animate-fadeOut px-4"
  >
    <img
      src="/favicon-rounded-centered.png"
      alt="ParkLink logo"
      class="w-40 h-40 sm:w-32 sm:h-32 animate-pulse"
    />
  </div>
</template>

<script setup>
import { onMounted } from "vue";

const emit = defineEmits(["finished"]);

onMounted(() => {
  setTimeout(() => {
    emit("finished");
  }, 3000);
});
</script>

<style scoped>
@keyframes fadeOut {
  0% {
    opacity: 1;
  }
  85% {
    opacity: 1;
  }
  100% {
    opacity: 0;
    display: none;
  }
}

.animate-fadeOut {
  animation: fadeOut 3s forwards;
}

/* Ajustes responsivos */
@media (max-width: 640px) {
  img {
    width: 120px !important;
    height: 120px !important;
  }
}
</style>
