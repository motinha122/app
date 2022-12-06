<template>
    <header class="bar">
        <slot></slot>  
        <h1 class="title">
            <slot name="title"></slot>
        </h1>
        <slot name="description"></slot>
    </header>
</template>

<script>

export default {
    data() {
        return {

        }
    },
}

</script>

<style>
.bar{
    color: white;
    background-color: black;
}
</style>