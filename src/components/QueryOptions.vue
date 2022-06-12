<script setup>
import { ref } from "vue";
import QueryField from "./QueryField.vue"

const title = ref('')
const cost = ref('')
const type = ref('')
const rules = ref('')
</script>

<template>
  <div class="flex flex-row items-center h-12 pl-2">
    <QueryField name="title" v-model="title" />
    <QueryField name="cost" v-model="cost" />
    <QueryField name="type" v-model="type" />
    <QueryField name="rules" v-model="rules" />
  </div>
</template>

<style scoped>
</style>
