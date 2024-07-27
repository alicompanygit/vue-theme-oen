<template>
    <h2 class="title fw-bold" v-html="text"></h2>
</template>
<script setup>
import { ref, defineProps, onMounted } from 'vue';
const props = defineProps({
  text: {
    typeof: String,
    default: 'title: lorem ipsum'
  },
  classes: {
    typeof: Array,
    default: []
  },
  color: {
    typeof: String,
    default: 'black'
  },
  size: {
    typeof: String,
    default: null
  }
});
onMounted(() => {
  for (let index = 0; index < props.classes.length; index++) {
    document.querySelectorAll(".title").forEach((el) => {
      el.classList.add(props.classes[index])
    })
  }
  document.querySelectorAll(".title").forEach((el) => {
    el.style.background = props.color;
    el.style.webkitBackgroundClip = 'text'
    el.style.webkitTextFillColor = 'transparent'
    el.style.fontSize = props.size
  })
})
</script>
<style scoped></style>