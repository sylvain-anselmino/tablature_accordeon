<script setup>
import Bouton from "./Bouton.vue";
defineProps({
  currentNotes: {
    type: Array
  }
});
</script>

<template>
  <div class="container">
    <Bouton pousse="Fa#" tire="Do" :current-notes="currentNotes">11</Bouton>
    <Bouton pousse="Fa" tire="Do#" :currentNotes="currentNotes">10</Bouton>
    <Bouton pousse="Mib" tire="Sib" :currentNotes="currentNotes">9</Bouton>
    <Bouton pousse="Fa#" tire="Sol" :currentNotes="currentNotes">8</Bouton>
    <Bouton pousse="Fa" tire="Mib" :currentNotes="currentNotes">7</Bouton>
    <Bouton pousse="Mib" tire="Do#" :currentNotes="currentNotes">6</Bouton>
    <Bouton pousse="Fa#?" tire="Sib" :currentNotes="currentNotes">5</Bouton>
    <Bouton pousse="Fa" tire="Sol" :currentNotes="currentNotes">4</Bouton>
    <Bouton pousse="Mib" tire="Mib" :currentNotes="currentNotes">3</Bouton>
    <Bouton pousse="Fa#?" tire="Do#" :currentNotes="currentNotes">2</Bouton>
    <Bouton pousse="Fa" tire="Sib" :currentNotes="currentNotes">1</Bouton>
  </div>
  <div class="container">
    <Bouton pousse="Sol" tire="Ré" :currentNotes="currentNotes">12</Bouton>
    <Bouton pousse="Mi" tire="Si" :currentNotes="currentNotes">11</Bouton>
    <Bouton pousse="Do" tire="Sol#" :currentNotes="currentNotes">10</Bouton>
    <Bouton pousse="La" tire="Fa" :currentNotes="currentNotes">9</Bouton>
    <Bouton pousse="Mi" tire="Ré" :currentNotes="currentNotes">8</Bouton>
    <Bouton pousse="Do" tire="Si" :currentNotes="currentNotes">7</Bouton>
    <Bouton pousse="La" tire="Sol#" :currentNotes="currentNotes">6</Bouton>
    <Bouton pousse="Mi" tire="Fa" :currentNotes="currentNotes">5</Bouton>
    <Bouton pousse="Do" tire="Ré" :currentNotes="currentNotes">4</Bouton>
    <Bouton pousse="La" tire="Si" :currentNotes="currentNotes">3</Bouton>
    <Bouton pousse="Sib" tire="Sol#" :currentNotes="currentNotes">2</Bouton>
    <Bouton pousse="Mi" tire="Sol" :currentNotes="currentNotes">1</Bouton>
  </div>
  <div class="container" >
    <Bouton pousse="Ré" tire="La" :currentNotes="currentNotes">11</Bouton>
    <Bouton pousse="Si" tire="Fa#" :currentNotes="currentNotes">10</Bouton>
    <Bouton pousse="Sol" tire="Mi" :currentNotes="currentNotes">9</Bouton>
    <Bouton pousse="Ré" tire="Do" :currentNotes="currentNotes">8</Bouton>
    <Bouton pousse="Si" tire="La" :currentNotes="currentNotes">7</Bouton>
    <Bouton pousse="Sol" tire="Fa#" :currentNotes="currentNotes">6</Bouton>
    <Bouton pousse="Ré" tire="Mi" :currentNotes="currentNotes">5</Bouton>
    <Bouton pousse="Si" tire="Do" :currentNotes="currentNotes">4</Bouton>
    <Bouton pousse="Sol" tire="La" :currentNotes="currentNotes">3</Bouton>
    <Bouton pousse="Ré" tire="Fa#" :currentNotes="currentNotes">2</Bouton>
    <Bouton pousse="Mib" tire="Mi" :currentNotes="currentNotes">1</Bouton>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 0 10px;
}
</style>
