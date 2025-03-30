<script setup>

defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="greetings">
    <h1>{{ msg }}</h1>
    <h3>
      Welcome! To get started, make sure you have music locally stored.
      Consider visiting my <a href = "https://matthew-sporman.github.io"  target="_blank" rel="noopener noreferrer">portfolio</a> to see my other works!
    </h3>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Boldonse&display=swap');

h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
  color: black;
  font-family: "Boldonse", system-ui;
  font-weight: 400;
  font-style: normal;
}

h3 {
  font-size: 1.0rem;
  font-family: "Boldonse", system-ui;
}

.greetings h1,
.greetings h3 {
  text-align: center;
  padding: 20px;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: center;
  }
}
</style>