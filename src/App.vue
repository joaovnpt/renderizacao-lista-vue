<script setup>
import { computed, ref } from 'vue'
const cidades = ref([
  'São Paulo',
  'Rio de Janeiro',
  'Belo Horizonte',
  'Salvador',
  'Fortaleza',
  'Curitiba',
  'Manaus',
  'Recife',
  'Porto Alegre',
  'Brasília'
])
const cidadesSort = computed(() => cidades.value.sort())
</script>

<template>
  <ul>
    <li v-for="(cidade, index) in cidadesSort" :key="index">{{ cidade }}</li>
  </ul>
</template>

<style scoped></style>
