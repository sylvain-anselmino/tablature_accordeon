<script setup>
import { ref } from "vue";
let selected = ref(false);
</script>
<template>
  <div class="item" 
  :class="{red : selected}"
  @click="selected = ! selected; $event.reset = !selected">
    <i>
      <slot></slot>
    </i>
  </div>
</template>

<style scoped>
.item {
  border: solid 1px gray;
  border-radius: 5px;
  min-width:  60px;
  height: 60px;
  text-align: center;
  cursor: pointer;
}
.red{
  background-color: brown;
}
</style>
