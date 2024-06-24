<template>
    <div class="container d-flex flex-column justify-content-start align-items-center main-content mt-5">
        <p class="fs-1">Home</p>
        <p class="fs-3">I love Hailey E. Young!</p>
        <TempComponent />
        <div>
            <p class="fs-3">My favourite stocks!</p>
            <div class="d-flex justify-content-between">
                <AmazonIcon />
                <AmdIcon />
                <AppleIcon />
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import TempComponent from '../components/TempComponent.vue';
import AmazonIcon from '../components/icons/amazon-icon.vue';
import AmdIcon from '../components/icons/amd-icon.vue';
import AppleIcon from '../components/icons/apple-icon.vue';
</script>

<style scoped>
</style>