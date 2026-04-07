<script setup>
import ModelParentComponent from './components/modelParentComponent.vue';
import ParentComponent from './components/parentComponent.vue';
</script>

<template>
    <p>Stap 1: Werken met defineProps en defineEmits</p>
    <ParentComponent />

    <b>Stap 2: Werken met defineModel</b>
    <ModelParentComponent />
</template>
