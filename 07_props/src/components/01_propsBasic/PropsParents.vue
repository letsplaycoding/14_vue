<template>
    <div>
        props 입력: <input v-model="message"/>
        <PropsChild :message="message"/>
        <DarkMode @toggle="toggleDarkMode"/>
    </div>
</template>

<script setup>
    import { ref } from 'vue'
    import PropsChild from './PropsChild.vue';
    import DarkMode from './DarkMode.vue';

    const message = ref('Good Game.');
</script>

<style scoped>
    .container{
        border: 1px solid black;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .dart {
        background-color: black;
        color: white;
    }
</style>