<template>
    <div :class="baseClass">
        <slot></slot>
        <button @click="onClick()">
            X
        </button>
    </div>
</template>

<script>
export default {
    props: {
        variant: {
            type: String,
            default: ''
        }
    },
    computed: {
        baseClass() {
            return [
                'alert',
                this.variant ? `alert-${this.variant}` : ''
            ]
        }
    },
    methods: {
        onClick() {
            this.$emit('close')
            console.log('closed')
        }
    }
}
</script>

<style scoped>
.alert {
    display: flex;
    padding: 5px;
    width: 90%;
    border-radius: 6px;
    color: gray;
    background: #dddddd;
}

.alert-success {
    background: #42b983;
    color: #ffffff;
}

button {
    margin-left: auto;
}
</style>