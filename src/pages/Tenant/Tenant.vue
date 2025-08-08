<template>
  <v-container>
    <v-card>
      <v-tabs v-model="tab" background-color="primary" dark>
        <v-tab value="users">Usuários</v-tab>
        <!-- Adicione outras abas aqui se quiser -->
      </v-tabs>
      <v-window v-model="tab">
        <v-window-item value="users">
          <v-card flat>
            <v-card-title>Usuários do Tenant</v-card-title>
            <v-card-text>
              <!-- Conteúdo da aba Usuários -->
              <v-list>
                <v-list-item v-for="user in users" :key="user.id">
                  <v-list-item-title>{{ user.name }}</v-list-item-title>
                  <v-list-item-subtitle>{{ user.email }}</v-list-item-subtitle>
                </v-list-item>
              </v-list>
            </v-card-text>
          </v-card>
        </v-window-item>
      </v-window>
    </v-card>
  </v-container>
</template>

<script setup>
import { ref } from 'vue'

const tab = ref('users')
const users = ref([
  { id: 1, name: 'Alice', email: 'alice@email.com' },
  { id: 2, name: 'Bob', email: 'bob@email.com' },
])
</script>