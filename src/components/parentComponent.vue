<template>
    <childComponent @update-message="handleMessage" :message="initialMessage" />
    <p>Recent bericht: {{ message }}</p>
</template>

<script setup>
import {ref} from 'vue';
import childComponent from './childComponent.vue';

const initialMessage = 'Hallo Vue 3!';
const message = ref('');

const handleMessage = newMessage => {
    message.value = newMessage;
};
</script>
