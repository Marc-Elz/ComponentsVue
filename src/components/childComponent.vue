<template>
    <div>
        <h3>{{ message }}</h3>
    </div>
    <button @click="emitEvent">Nieuw bericht</button>
</template>

<script setup>
// Props
defineProps({
    message: String,
});

// emit
const emit = defineEmits(['updateMessage']);

const emitEvent = () => {
    emit('updateMessage', 'bericht van kindcomponent');
};
</script>
