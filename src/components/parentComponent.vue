<template>
    <childComponent :message="title" />
    <childComponent :message="message" />
</template>

<script setup>
import childComponent from './childComponent.vue';

const title = 'Welkom in Vue 3';
const message = 'Hallo Vue 3!';
</script>
