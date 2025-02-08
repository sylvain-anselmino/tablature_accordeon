<script setup>
import AccordItem from "./AccordItem.vue";
const emit = defineEmits(['select-accord']);

function sendNotes(args){
  emit('select-accord', args)
}
</script>

<template>
  <div class="container">
      <AccordItem @click="$event.reset ?  sendNotes([]) : sendNotes(['Do', 'Mi', 'Sol'])">C</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Do', 'Mib', 'Sol'])">Cm</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Ré', 'Fa#', 'La'])">D</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Ré', 'Fa', 'La'])">Dm</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Mi', 'Sol#', 'Si'])">E</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Mi', 'Sol', 'Si'])">Em</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Fa', 'La', 'Do'])">F</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Fa', 'Sol#', 'Do'])">Fm</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Sol', 'Si', 'Ré'])">G</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Sol', 'Sib', 'Ré'])">Gm</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['La', 'Do#', 'Mi'])">A</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['La', 'Do', 'Mi'])">Am</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Si', 'Ré#', 'Fa#'])">B</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Si', 'Ré', 'Fa#'])">Bm</AccordItem>
  </div>

</template>
<script>


</script>

<style scoped>
.container {
  display: flex;
  flex-wrap: wrap;
  flex: 1 1 50%; /* Chaque élément occupe 50% de la largeur du conteneur */
  padding: 10px; /* Optionnel : pour ajouter de l'espace autour des éléments */
}
</style>
