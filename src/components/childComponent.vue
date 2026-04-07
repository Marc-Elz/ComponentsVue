<template>
    <div>
        <h3>{{ message }}</h3>
    </div>
</template>

<script setup>
defineProps({
    message: String,
});
</script>
