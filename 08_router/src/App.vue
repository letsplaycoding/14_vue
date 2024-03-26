<script setup>
  import { RouterLink, RouterView } from 'vue-router';

</script>

<template>
  <header>
    <h1>Router 사용하기</h1>
    <hr>
    <div class="wrapper">
      <h2>basic router</h2>
      <nav>
        <RouterLink to="/">Home</RouterLink>
      </nav>
    </div>
  </header>

  <main>
    <RouterView/>
  </main>
</template>

<style scoped>

</style>
