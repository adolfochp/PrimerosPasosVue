<template>
    <div class="post">
        <h3>{{ props.title }}</h3>
        <p>{{ props.content }}</p>
        <button @click="handleClick()">Diii Hola</button>
        <input type="text" v-model ="message"/>
    </div>
    
</template>

<script>
import { defineComponent,ref } from 'vue';
export default defineComponent({
    name:'PostDetail',
    props:{
        title:{
            type:String,
            required:true
        },
        content:{
            type:String,
            required:false,
            default:"Este post no tiene contenido"
        }
    },
    emits:["sayHi"],
    setup(props,{emit}){
        const handleClick=()=>{
            emit("sayHi",message.value)
        }
        let message=ref('')
         return {props,message,handleClick}

    }
})
</script>
<style scoped>
.post{
    width: 300px;
    height: 200px;
    background-color: aqua;
    border-radius: 20px;
    margin: 10px;
    padding: 10px;
}
</style>
