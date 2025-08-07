<template>
  <v-app>
    <v-layout>

      <!-- Navigation Drawer -->
      <NavigationDrawer />

      <!-- App Content -->
      <v-main>
        <v-container fluid>
          <v-card>
            <v-card-title>Conteúdo principal</v-card-title>
            <v-card-text>
              O conteúdo se ajusta automaticamente ao tamanho do drawer.
            </v-card-text>
          </v-card>
        </v-container>
      </v-main>

    </v-layout>
  </v-app>
</template>

<script setup>
import { ref } from 'vue'

const drawer = ref(true)
const rail = ref(true)
</script>
       