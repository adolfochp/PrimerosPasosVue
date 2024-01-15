<template>
  <!-- <p :class="{ 'danger':hasError}"> Mensaje enviado satisfactoriamente...</p>   -->
<p v-bind:style="{ backgroundColor:'#ccc',color:c}">Mensaje enviado satisfactoriamente....</p> 
<button v-on:click="handleClick">Cambiar color</button>
</template>
<!-- <script >
  import { defineComponent } from 'vue';
  export default defineComponent({
    name:'ClassBind',
    setup(){
        let hasError =true;
        return{hasError}
    }
  })
<script setup>
  let hasError =true;
</script> -->
 <script setup>
 import{ref} from 'vue'
  let c=ref ('#fff');
  const handleClick =()=>c.value= '#ff0000'
 
</script> 
<!-- <script >
  import { defineComponent } from 'vue';
  export default defineComponent({
    name:'ClassBind',
    data(){
        return{
            hasError:true
        }
    }
  })
</script>
 -->


<style scoped>

</style>