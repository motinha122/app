<template>
    <div :class="baseClass">
        <slot></slot>
        {{test}}
    </div>
</template>

<script>
export default {
    props: {
        variant:{
            type:String,
            default: ''
        },
        test:{
            type: String,
            default:'test'
        },
    },
    computed: {
        baseClass() { // return 'alert alert-variant' or 'alert'
            return [
                'alert',
                this.variant ? `alert-${this.variant}` : ''
            ]
        }
    }
}
</script>

<style scoped>
.alert {
    padding: 5px;
    width: fit-content;
    border-radius: 6px;
    color: gray;
    background: #dddddd;
}
.alert-success {
    background: #42b983;
    color: #ffffff;
}
</style>