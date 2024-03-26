<template>
    <h1>child: {{ injectCount }}</h1>
    <GrandChild/>
</template>

<script setup>
    import { inject } from 'vue';
    import GrandChild from './DrillingGrandChild.vue';

    const injectCount = inject('count');
</script>