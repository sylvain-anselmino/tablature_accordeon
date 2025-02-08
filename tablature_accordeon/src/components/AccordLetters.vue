<script setup>
import AccordItem from "./AccordItem.vue";
</script>

<template>
  <div class="container">
      <AccordItem @click="$emit('select-accord', ['Do', 'Mi', 'Sol'])">C</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Do', 'Mib', 'Sol'])">Cm</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Ré', 'Fa#', 'La'])">D</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Ré', 'Fa', 'La'])">Dm</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Mi', 'Sol#', 'Si'])">E</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Mi', 'Sol', 'Si'])">Em</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Fa', 'La', 'Do'])">F</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Fa', 'Sol#', 'Do'])">Fm</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Sol', 'Si', 'Ré'])">G</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Sol', 'Sib', 'Ré'])">Gm</AccordItem>
      <AccordItem @click="$emit('select-accord', ['La', 'Do#', 'Mi'])">A</AccordItem>
      <AccordItem @click="$emit('select-accord', ['La', 'Do', 'Mi'])">Am</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Si', 'Ré#', 'Fa#'])">B</AccordItem>
      <AccordItem @click="$emit('select-accord', ['Si', 'Ré', 'Fa#'])">Bm</AccordItem>
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
