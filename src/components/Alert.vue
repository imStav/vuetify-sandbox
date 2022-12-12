<script setup>
defineProps({
    status: {
        type: String,
        required: true,
    },
    message: {
        type: String,
        required: true,
    }
})
</script>

<template>
<v-alert
    :color="status ? 'default' : 'info'"
    variant="tonal"
    density="compact"
>
    {{ message }}
</v-alert>
</template>