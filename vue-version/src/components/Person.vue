<script setup>

import { defineProps } from 'vue'

defineProps({
    person: Object
})
// console.log(person);
</script>
<template>
    <article>
        <img :src="person.image" alt="">
        <div>
            <h2>{{  person.name }}</h2>
            <p>{{ person.age }} years old</p>
        </div>
    </article>
</template>

<style>
    article {
        display: flex;
        margin: 1rem 0;
        padding: 1rem;
        border-radius: 0.5rem;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    img {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        margin-right: 1rem;
    }

    h2 {
        margin: 0;
    }

    p {
        margin: 0.5rem 0;
    }
</style>