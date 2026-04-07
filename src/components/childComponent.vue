<template>
    <div>
        <h3>{{ message }}</h3>
    </div>
    <button @click="emitEvent">Nieuw bericht</button>
</template>

<script setup>
defineProps({
    message: String,
});

const emit = defineEmits(['updateMessage']);

const emitEvent = () => {
    emit('updateMessage', 'bericht van kindcomponent');
};
</script>
