<template>
    <div class="border p-4">
        <p>This is a temp component!</p>
        <p>{{ tempCount }}</p>
        <p>{{ tempProp }}</p>
        <button class="btn btn-primary" @click="increaseTempCount">+</button>
        <button class="btn btn-warning" @click="decreaseTempCount">-</button>
        <LoadingIndicator />
    </div>
</template>

<script setup lang="ts">
import { withDefaults } from 'vue';
import { storeToRefs } from 'pinia';
import { useTempStore } from '@/stores/TempStore';
import LoadingIndicator from './loading/LoadingIndicator.vue';

const props = withDefaults(defineProps<{
    tempProp?: string,
}>(), {
    tempProp: "tempValue",
});
    
// access tempProp through props.tempProp.value

const { increaseTempCount, decreaseTempCount } = useTempStore();
const { tempCount } = storeToRefs(useTempStore());
</script>

<style scoped>
</style>
