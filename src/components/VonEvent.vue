<template>
    <div>
        <button v-on:click="onclick">
            Send
        </button>
        <button @click="onclick">
            Send
        </button>
    </div>
    <div @mouseover="onMouse" class="a">A</div>
    <form action="https://google.com" @submit="onSubmit">
        <button type="submit">
            Send
        </button>
    </form>
    <input type="text" @keyup="onKeyUp">

</template>

<script>

export default{
    data(){
        return {
            
        }
    },
    methods:{
        onclick(){
            console.log('xampson');
        },
        onMouse(){
            console.log('mouse over');
        },
        onKeyUp(evt){
            console.log('onKeyUp',evt)
        }
    }
}

</script>

<style>
.a{
    text-align: center;
    width: 40px;
    height: 40px;
    border: 2px solid black;
}
</style>