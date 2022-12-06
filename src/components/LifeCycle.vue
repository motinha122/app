<template>
    <div>
        <h1>Goodbye World</h1>
        {{name}}
    </div>
</template>
 
<script>

export default {
    data() {
        return {
            name:'Xampson',
        }
    },
    beforeCreate() {
        console.log('beforeCreate');
    },
    created() {
        console.log('created');
        console.log(this.name);
    },
    beforeMount() {
        console.log('beforeMount');
    },
    mounted() {
        console.log('mounted');
        console.log(this.$el);
    },
    beforeUnmount() {
        console.log('beforeUnmount');
    },
    unmounted() {
        console.log('unmounted');
    },
    watch: {

    },
    methods: {

    },
    computed: {

    }
}

</script>
 
<style>

</style>