<template>
    
</template>

<script setup>
    import { provide } from 'vue';

    const count = ref(0);
    provide('count', count);        // provide를 통해 별도의 공간에 count 반응형 변수값을 'count'라는 이름으로 담아둠
</script>

<style scoped>

</style>