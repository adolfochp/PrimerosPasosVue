<template>
    <div> hola mundo</div>
    
</template>

<script>

import {defineComponent} from 'vue'

export default defineComponent({
    name:"CycleOption",
    created(){
        console.log("created");

    },
    updated(){
        console.log("updated");

    },
    mounted(){
        console.log("mounted");

    },
    unmounted(){
        console.log("unmountd");

    },
})

</script>
<style scoped>

</style>
