<template>
    <h2 v-if="age<18">Eres menor de edad</h2>
    <h3 v-else>Eres mayor de edad</h3>
    <h1 v-show="age<18">Eres menor de edad</h1>
    <h1 v-show="age>=18">Eres mayor de edad</h1>
</template>

<script setup>
   let age=11
</script>

<style scoped>

</style>
