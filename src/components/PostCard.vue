<template>
    <div  class ='post-card'>
        <h3>Titulo </h3>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Velit architecto corporis sed natus molestiae maxime ea quasi? Quos, laboriosam minus id exercitationem repudiandae ullam autem voluptas, harum temporibus dolores obcaecati.</p>
        <PostButton />
        <CounterOption/>

   
    </div>
    
</template>

<script setup>
import PostButton from './PostButton.vue'
import CounterOption from './CounterOption.vue';
</script>
<style scoped>
.post-card{
    border-radius:15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;

}

</style>
