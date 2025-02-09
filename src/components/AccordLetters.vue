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

      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Do#', 'Fa', 'Sol#'])">C# ou Db</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Do#', 'Mi', 'Sol#'])">C#m ou Dbm</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Ré', 'Fa#', 'La'])">D</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Ré', 'Fa', 'La'])">Dm</AccordItem>

      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Mib', 'Sol', 'Sib'])">D# ou Eb</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Mib', 'Fa#', 'Sib'])">D#m ou Ebm</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Mi', 'Sol#', 'Si'])">E</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Mi', 'Sol', 'Si'])">Em</AccordItem>

      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Fa', 'La', 'Do'])">F</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Fa', 'Sol#', 'Do'])">Fm</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Fa#', 'Sib', 'Do#'])">F# ou Gb</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Fa#', 'La', 'Do#'])">F#m ou Gbm</AccordItem>

      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Sol', 'Si', 'Ré'])">G</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Sol', 'Sib', 'Ré'])">Gm</AccordItem>

      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Sol#', 'Do', 'Mib'])">G# ou Ab</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Sol#', 'Si', 'Mib'])">G#m ou Abm</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['La', 'Do#', 'Mi'])">A</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['La', 'Do', 'Mi'])">Am</AccordItem>

      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Sib', 'Ré', 'Fa'])">A# ou Bb</AccordItem>
      <AccordItem @click="$event.reset ?  sendNotes([]) :sendNotes( ['Sib', 'Do#', 'Fa'])">A#m ou Bbm</AccordItem>
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
