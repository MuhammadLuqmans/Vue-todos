<script setup lang="ts">
import TodosVue from '@/components/Todos/Todos.vue';
</script>

<template>
  <div class="about">
    <TodosVue />
  </div>
</template>

<style >
.about{
  background: pink;
  height: 100vh;
  width:100%;
  font-family: "'Roboto', sans-serif";
  margin: auto;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>