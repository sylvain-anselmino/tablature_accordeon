<script setup>
import { ref } from "vue";
import LetterNotes from "./components/AccordLetters.vue";
import Clavier from "./components/Clavier.vue";

let currentNotes = ref([]);
</script>

<template>
  <header></header>

  <main>
    <div class="container">
      <Clavier :current-notes="currentNotes" />
      <div class="separatorV"></div>

      <LetterNotes @select-accord="currentNotes = $event" />
    </div>

    <div style="width: 400px">
      <h1>Accords Majeurs</h1>
      <div>Do majeur (C) : Do, Mi, Sol</div>
      <div>Ré♭ majeur (D♭) : Ré♭, Fa, La♭</div>
      <div>Ré majeur (D) : Ré, Fa#, La</div>
      <div>Mi♭ majeur (E♭) : Mi♭, Sol, Si♭</div>
      <div>Mi majeur (E) : Mi, Sol#, Si</div>
      <div>Fa majeur (F) : Fa, La, Do</div>
      <div>Sol♭ majeur (G♭) : Sol♭, Si♭, Ré♭</div>
      <div>Sol majeur (G) : Sol, Si, Ré</div>
      <div>La♭ majeur (A♭) : La♭, Do, Mi♭</div>
      <div>La majeur (A) : La, Do#, Mi</div>
      <div>Si♭ majeur (B♭) : Si♭, Ré, Fa</div>
      <div>Si majeur (B) : Si, Ré#, Fa#</div>
      <h1>Accords Mineurs</h1>
      <div>Do mineur (Cm) : Do, Mib, Sol</div>
      <div>Ré♭ mineur (D♭m) : Ré♭, Fa♭, La♭</div>
      <div>Ré mineur (Dm) : Ré, Fa, La</div>
      <div>Mi♭ mineur (E♭m) : Mi♭, Sol♭, Si♭</div>
      <div>Mi mineur (Em) : Mi, Sol, Si</div>
      <div>Fa mineur (Fm) : Fa, Lab, Do</div>
      <div>Sol♭ mineur (G♭m) : Sol♭, Si♭♭, Ré♭</div>
      <div>Sol mineur (Gm) : Sol, Sib, Ré</div>
      <div>La♭ mineur (A♭m) : La♭, Do♭, Mi♭</div>
      <div>La mineur (Am) : La, Do, Mi</div>
      <div>Si♭ mineur (B♭m) : Si♭, Ré♭, Fa</div>
      <div>Si mineur (Bm) : Si, Ré, Fa#</div>
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
