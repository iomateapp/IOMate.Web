<template>
  <v-card>
    <v-card-title>Usuários</v-card-title>
    <v-card-text>
      Aqui você pode gerenciar os usuários do sistema.
    </v-card-text>
  </v-card>
</template>

<script setup>
import { ref } from 'vue'

const users = ref([
  { id: 1, name: 'John Doe', email: 'john.doe@example.com' },
  { id: 2, name: 'Jane Smith', email: 'jane.smith@example.com' },
  { id: 3, name: 'Alice Johnson', email: 'alice.johnson@example.com' },
])
</script>

<style scoped>
/* Add any specific styles for the Users page here */
</style>