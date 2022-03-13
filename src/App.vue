<template>
  <v-app>
    <v-main>
      <h1>My Parent component timeline</h1>
      <v-timeline direction="horizontal" density="compact" truncate-line="both">
        <v-timeline-item
          v-for="item in items"
          :key="item.id"
          :dot-color="item.color"
          size="small"
          fill-dot
        >Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.</v-timeline-item>
      </v-timeline>
      <h1>My Child component Timeline</h1>
      <my-timeline></my-timeline>
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
import { reactive } from 'vue';
import MyTimeline from './components/MyTimeline.vue';
const items = reactive([
  {
    id: 1,
    color: 'info',
    icon: 'mdi-information',
  },
  {
    id: 2,
    color: 'info',
    icon: 'mdi-alert-circle',
  }, {
    id: 3,
    color: 'error',
    icon: 'mdi-alert-circle',
  }, {
    id: 4,
    color: 'error',
    icon: 'mdi-alert-circle',
  },
])
</script>
