<script setup>
import { ref } from "vue";
import LetterNotes from "./components/LetterNotes.vue";
import Clavier from "./components/Clavier.vue";

let currentNotes = ref([]);
</script>

<template>
  <header></header>

  <main>
    <div class="container">
      <Clavier :current-notes="currentNotes" />
      <div class="separatorV"></div>
      <LetterNotes @select-accord="currentNotes=$event" />
    </div>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.container {
  display: flex;
  justify-content: center;
}
header {
  display: flex;
  place-items: center;
  padding-right: calc(var(--section-gap) / 2);
}
.separatorV {
  width: 100px;
}
</style>
