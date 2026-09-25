<script setup>
    defineEmits(['on-input']);
</script>

<template>
    <input type="text" placeholder="Enter your name" @input="$emit('on-input')" />
</template>

<style scoped>
</style>
