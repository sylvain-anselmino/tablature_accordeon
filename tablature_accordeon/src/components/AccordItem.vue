<script setup>
</script>
<template>
  <div class="item">
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
</style>
