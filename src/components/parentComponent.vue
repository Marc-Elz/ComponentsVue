<template>
    <childComponent :message="message" />
</template>

<script setup>
import childComponent from './childComponent.vue';

const message = 'Hallo Vue 3!';
</script>
