<script setup>
import {ref} from 'vue'
const people = ['Wade Cooper', 'Arlene Mccoy', 'Devon Webb', 'Tom Cook', 'Tanya Fox', 'Hellen Schmidt', 'Caroline Schultz', 'Mason Heaney', 'Claudie Smitham', 'Emil Schaefer']

const selected = ref(people[0])
</script>

<template>
  <SSelectMenu v-model="selected" :options="people" />
</template>
