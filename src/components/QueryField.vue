<script setup>
import { ref } from "vue";

defineProps({
  name: String
})

const input = ref("")
</script>

<template>
  <h1 class="capitalize">{{ name }}</h1>
  <input class="ml-4 mr-10 px-1 rounded text-zinc-800" type="text" v-model="input" @input="$emit('update:modelValue', $event.target.value)" />
</template>

<style scoped>
</style>
