  <script setup>
    import {ref} from "vue";
    const count = ref(0) ;
  </script>

<template>
  <main>
  <div>
    <h3>the current count is ...</h3>
    <h1>{{ count }}</h1>
    <button v-on:click="count--">-</button>
    <button @click="count++">+</button>
  </div>
</main>
</template>

<style scoped>
  main {
    background-color: aliceblue;
    height: 100vh;
    width: 100vw;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  div {
    text-align: center;
  }

</style>