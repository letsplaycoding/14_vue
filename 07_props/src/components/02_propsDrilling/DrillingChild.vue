<template>
    <h1>child: {{ injectCount }}</h1>
</template>

<script setup>
    import { inject } from 'vue';

    const injectCount = inject('count');
</script>