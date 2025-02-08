<script setup>
import WelcomeItem from "./NoteItem.vue";
</script>

<template>
  <div class="container">
    <WelcomeItem @click="$emit('select-accord', [])">Effacer</WelcomeItem>
    <div>
      <WelcomeItem @click="$emit('select-accord', ['Do', 'Mi', 'Sol'])"
        >C</WelcomeItem
      >
      <WelcomeItem @click="$emit('select-accord', ['Do', 'Mib', 'Sol'])"
        >Cm</WelcomeItem
      >
    </div>
    <div>
      <WelcomeItem @click="$emit('select-accord', ['Ré', 'Fa#', 'La'])">D</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Ré', 'Fa', 'La'])">Dm</WelcomeItem>
    </div>
    <div>
      <WelcomeItem @click="$emit('select-accord', ['Mi', 'Sol#', 'Si'])">E</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Mi', 'Sol', 'Si'])">Em</WelcomeItem>
    </div>
    <div>
      <WelcomeItem @click="$emit('select-accord', ['Fa', 'La', 'Do'])">F</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Fa', 'Sol#', 'Do'])">Fm</WelcomeItem>
    </div>
    <div>
      <WelcomeItem @click="$emit('select-accord', ['Sol', 'Si', 'Ré'])">G</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Sol', 'Sib', 'Ré'])">Gm</WelcomeItem>
  </div>
    <div>
      <WelcomeItem @click="$emit('select-accord', ['La', 'Do#', 'Mi'])">A</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['La', 'Do', 'Mi'])">Am</WelcomeItem>
  </div>
    <div>
      <WelcomeItem @click="$emit('select-accord', ['Si', 'Ré#', 'Fa#'])">B</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Si', 'Ré', 'Fa#'])">Bm</WelcomeItem>
    </div>
  </div>

  <div class="container" style="width: 400px">
    <h1>Accords Majeurs</h1>
    <div>Do majeur (C) : Do, Mi, Sol</div>
    <div>Ré majeur (D) : Ré, Fa#, La</div>
    <div>Mi majeur (E) : Mi, Sol#, Si</div>
    <div>Fa majeur (F) : Fa, La, Do</div>
    <div>Sol majeur (G) : Sol, Si, Ré</div>
    <div>La majeur (A) : La, Do#, Mi</div>
    <div>Si majeur (B) : Si, Ré#, Fa#</div>
    <h1>Accords Mineurs</h1>
    <div>Do mineur (Cm) : Do, Mib, Sol</div>
    <div>Ré mineur (Dm) : Ré, Fa, La</div>
    <div>Mi mineur (Em) : Mi, Sol, Si</div>
    <div>Fa mineur (Fm) : Fa, Lab, Do</div>
    <div>Sol mineur (Gm) : Sol, Sib, Ré</div>
    <div>La mineur (Am) : La, Do, Mi</div>
    <div>Si mineur (Bm) : Si, Ré, Fa#</div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.container>div {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>
