<script setup>
import {ref} from 'vue'

const countries = ['United States', 'Canada', 'Mexico']

const country = ref(countries[0])
</script>

<template>
  <SSelect v-model="country" :options="countries"/>
</template>
