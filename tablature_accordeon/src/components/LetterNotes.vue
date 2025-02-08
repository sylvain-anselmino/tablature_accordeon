<script setup>
import WelcomeItem from "./NoteItem.vue";
</script>

<template>
    <div><button @click="$emit('select-accord', [])">Effacer</button></div>
  <div class="container">
      <WelcomeItem @click="$emit('select-accord', ['Do', 'Mi', 'Sol'])"
        >C</WelcomeItem
      >
      <WelcomeItem @click="$emit('select-accord', ['Do', 'Mib', 'Sol'])"
        >Cm</WelcomeItem
      >
      <WelcomeItem @click="$emit('select-accord', ['Ré', 'Fa#', 'La'])">D</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Ré', 'Fa', 'La'])">Dm</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Mi', 'Sol#', 'Si'])">E</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Mi', 'Sol', 'Si'])">Em</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Fa', 'La', 'Do'])">F</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Fa', 'Sol#', 'Do'])">Fm</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Sol', 'Si', 'Ré'])">G</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Sol', 'Sib', 'Ré'])">Gm</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['La', 'Do#', 'Mi'])">A</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['La', 'Do', 'Mi'])">Am</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Si', 'Ré#', 'Fa#'])">B</WelcomeItem>
      <WelcomeItem @click="$emit('select-accord', ['Si', 'Ré', 'Fa#'])">Bm</WelcomeItem>
  </div>

</template>

<style scoped>
.container {
  display: flex;
  flex-wrap: wrap;
  flex: 1 1 50%; /* Chaque élément occupe 50% de la largeur du conteneur */
  padding: 10px; /* Optionnel : pour ajouter de l'espace autour des éléments */
}
</style>
