<script>
import PlayPauseButton from "@/components/buttons/PlayPauseButton.vue";
import NextButton from "@/components/buttons/NextButton.vue";
import PreviousButton from "@/components/buttons/PreviousButton.vue";

export default {
  name: "MediaPlayer",
  components: { PlayPauseButton, NextButton, PreviousButton }
}
</script>

<template>
  <div class="player-container">
    <div class="song-details">
      <h2 class="song-title">Song Title</h2>
      <p class="artist-name">Artist Name</p>
    </div>
    <div class="playback-controls">
      <NextButton />
      <PlayPauseButton />
      <PreviousButton />
    </div>
    <div class="volume-slider">
      <input type="range" class="volume-slider" value="50">
    </div>
    <div class="volume-text">Volume</div>
  </div>
</template>

<style scoped>
.player-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  transform: scale(1.75);
  margin-top: 325px;
}

.playback-controls {
  padding: 15px;
}

.volume-slider {
  padding: 5px;
  transform: scale(1.25);
}

.volume-text {
  font-size: 8px;
}
</style>