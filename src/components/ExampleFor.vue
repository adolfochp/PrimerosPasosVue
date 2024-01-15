<template>
    <ul>
        <li v-for="country in countries" :key="country.code">{{country.name}}</li>

    </ul>
</template>

<script setup>
import {ref} from 'vue'
let countries =ref([
    {
        code:'es',
        name:'Spain'

    },
    {
        code:'fr',
        name:'France'

    },
    {
        code:'en',
        name:'Uk'

    },
    {
        code:'gr',
        name:'Germany'

    },
])
</script>

<style scoped>

</style>
