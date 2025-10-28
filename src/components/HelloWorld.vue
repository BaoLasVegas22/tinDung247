<template>
  <section>
    <p>{{ msg }}</p>
    <input v-model="name" placeholder="Type your name" />
    <p v-if="name">Hello, {{ name }} 👋</p>
  </section>
</template>

<script setup>
import { ref } from 'vue'
const props = defineProps({ msg: String })
const name = ref('')
const { msg } = props
</script>

<style scoped>
input { padding: 0.5rem; font-size: 1rem; margin-top: 0.5rem; }
</style>
