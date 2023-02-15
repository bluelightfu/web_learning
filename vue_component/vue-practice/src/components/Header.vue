<template>
    <header>
        <h1>{{title}}</h1>
        <Button @click="onClick()" text="Add Text" color="green"/>

    </header>
</template>

<script>
import Button from "./Button.vue"
    export default {
        name:'Header',
        props:['title'],
        components:{
            Button
        },
        methods:{
            onClick:function(){
                console.log("Click!")
            }
        }
    }
</script>

<style scoped>
    header {
        display:flex;
        justify-content: space-between;
        align-content: center;
        margin-bottom: 20px;
    }
</style>