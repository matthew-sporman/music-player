<script setup>
import { ref } from "vue";
import { Play as LucidePlay, Pause as LucidePause } from "lucide-vue-next";
const isPlaying = ref(false);

const togglePlay = () => {
  isPlaying.value = !isPlaying.value;
};
</script>

<template>
  <button @click="togglePlay" class="PlayPauseButton">
    <component :is="isPlaying ? LucidePause : LucidePlay" class="w-6 h-6 text-white" />
  </button>
</template>

<style scoped>
.PlayPauseButton {
  border-radius: 20px;
  padding: 10px;
  font-family: "Boldonse", system-ui;
}

.PlayPauseButton:hover {
  transition: 0.25s ease-in-out;
  background-color: darkgray;
}
</style>