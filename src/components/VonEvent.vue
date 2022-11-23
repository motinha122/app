<template>
    <div>
        <button v-on:click="onclick()">
            Send
        </button>
        <button @click="onclick()">
            Send
        </button>
    </div>
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
        }
    }
}

</script>

<style>

</style>