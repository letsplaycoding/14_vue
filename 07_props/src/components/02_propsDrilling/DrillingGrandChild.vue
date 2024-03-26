
<!-- 
    Parents (provide)   -> Child (count에서 inject)
                        -> GrandChild (count에서 inject)
-->

<template>
    <div>
        <h3>GrandChild: {{ injectCount }}</h3>
        <button @click="injectCount++">GrandChild가 증가(수정)</button>
    </div>
</template>

<script setup>
    import { inject } from "vue";

    const injectCount = inject("count");
</script>

<style scoped>

</style>