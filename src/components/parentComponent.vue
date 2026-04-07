<template>
    <childComponent @update-message="handleMessage" :message="initialMessage" />
    <p>Recent bericht: {{ message }}</p>
</template>

<script setup>
import {ref} from 'vue';
import childComponent from './childComponent.vue';

//Define Props :message (parent -> child)
const initialMessage = 'Hallo Vue 3!';

//Define Emits @updateMessage (child -> parent)
const message = ref('');

const handleMessage = newMessage => {
    message.value = newMessage;
};
</script>
