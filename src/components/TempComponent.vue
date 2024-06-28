<template>
    <div class="border p-4">
        <p>This is a temp component!</p>
        <p>{{ tempCount }}</p>
        <button class="btn btn-primary" @click="increaseTempCount">+</button>
        <button class="btn btn-warning" @click="decreaseTempCount">-</button>
        <LoadingIndicator />
    </div>
</template>

<script setup lang="ts">
import { storeToRefs } from 'pinia';
import { useTempStore } from '@/stores/TempStore';
import LoadingIndicator from './loading/LoadingIndicator.vue';

const { increaseTempCount, decreaseTempCount } = useTempStore();
const { tempCount } = storeToRefs(useTempStore());
</script>

<style scoped>
</style>