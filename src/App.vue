<script setup>
import ToolDescription from './components/ToolDescription.vue'
import ProductIcon from "@/components/icons/ProductIcon.vue";
import MediaPlayer from "@/components/MediaPlayer.vue";

</script>

<template>
  <header>
    <div class="wrapper">
      <ProductIcon />
      <ToolDescription msg="The Sporman Song Satchel"/>
      <ProductIcon />
    </div>
  </header>

  <MediaPlayer />

</template>

<style scoped>

.wrapper {
  margin-top: 125px;
}

header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 4);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    text-align: center;
  }
}
</style>
