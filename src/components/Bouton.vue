<script setup>
defineProps({
  pousse: {
    type: String,
    required: true,
  },
  tire: {
    type: String,
    required: true,
  },
  currentNotes: {
    type: Array
  }
});
</script>
<template>
  <div class="item">
    <div class="pousse" :class="{selected: currentNotes && currentNotes.some(n=>n==pousse)}">{{ pousse }}</div>
    <div class="tire"  :class="{selected: currentNotes && currentNotes.some(n=>n==tire)}">{{tire}}</div>
    <slot></slot>
  </div>
</template>

<style scoped>
.item {
  display: flex;
  align-items: center;
  width: 80px;
  height: 60px;
  text-align: center;
  cursor: pointer;
  margin: 10px;

}
.item div{
  height: 100%;
  width: 50%;
  padding: 15px 10px;
}
.item :first-child{
  border-right: solid 1px black;
}
.tire{
  border-top-right-radius: 40px;
  border-bottom-right-radius: 40px;
  background-color: lightgray;
  border: solid 1px gray;
  margin-right: 2px;
}
.pousse{
  border-top-left-radius: 40px;
  border-bottom-left-radius: 40px;
  border: solid 1px gray;
}
.selected{
  background-color: brown;
}
</style>
