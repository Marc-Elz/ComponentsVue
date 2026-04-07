<template>
    <modelChildComponent v-model="sharedMessage" />
    <p>Huidig bericht: {{ sharedMessage }}</p>
</template>

<script setup>
import {ref} from 'vue';
import modelChildComponent from './modelChildComponent.vue';

const sharedMessage = ref('');
</script>
