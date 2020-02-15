<template>
  <img src="./assets/logo.png" alt="logo">
  <h1>Hello Vue 3 x TypeScript!</h1>
  <button @click="inc">Clicked {{ count }} times.</button>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  setup() {
    const count = ref(0)
    const inc = () => {
      count.value++
    }

    return {
      count,
      inc
    }
  }
})
</script>

<style scoped>
img {
  width: 200px;
}

h1 {
  font-family: Arial, Helvetica, sans-serif;
}
</style>
