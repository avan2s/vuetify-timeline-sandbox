<template>
    <v-timeline single-side="after" direction="horizontal" density="compact" truncate-line="true">
        <v-timeline-item
            v-for="item in items"
            :key="item.id"
            :dot-color="item.color"
            size="small"
            fill-dot
        >Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.</v-timeline-item>
    </v-timeline>
</template>
<script setup lang="ts">
import { reactive } from 'vue';

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