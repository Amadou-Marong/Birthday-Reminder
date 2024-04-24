<script setup>
    import Person from './Person.vue';
    defineProps({
        people: Object
    })
</script>
<template>
    <section>
        <div v-for="person in people" :key="person.id">
            <Person :person="person" />
        </div>
    </section>
</template>