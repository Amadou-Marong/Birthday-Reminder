<script setup>
  import { ref } from 'vue'
  import  data from './data'
  import List from './components/List.vue';
  
  const people = ref(data)
</script>

<template>
  <main>
    <section>
      <h3>{{ people.length }} Birthdays</h3>
      <List :people="people" />
      <button class="btn btn-block" @click="people.length = 0">Clear All</button>
    </section>
  </main>
</template>

