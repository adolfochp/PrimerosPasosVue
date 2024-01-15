<template>
    <form>
        <input type="text" v-model ="inputText"/>
        <input type="checkbox" v-model="agree"/> Acepto los terminos y condiciones
        <select v-model="country">
            <option>Spain</option>
            <option>Uk</option>
            <option>France</option>
        </select>
    </form>
    <h3>{{inputText}}</h3>
</template>

<script setup >
import {ref} from 'vue'
 let inputText=ref('')
 let agree=ref('')
 let country=ref('Spain')
//import {defineComponent}from 'vue'
//  export default defineComponent({
//     data(){
//         return{
//             inputText :'',
//             agree: true
//         }
            
//     }  
//     })

</script>
<style scoped>

</style>
