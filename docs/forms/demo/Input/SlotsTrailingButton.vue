<script setup lang="ts">
import {ref} from 'vue'

const q = ref('')
</script>

<template>
  <SInput v-model="q" name="q" placeholder="Search..." icon="i-heroicons-magnifying-glass-20-solid" :ui="{ icon: { trailing: { pointer: '' } } }">
    <template #trailing>
      <SButton
          v-show="q !== ''"
          color="gray"
          variant="link"
          icon="i-heroicons-x-mark-20-solid"
          :padded="false"
          @click="q = ''"
      />
    </template>
  </SInput>
</template>