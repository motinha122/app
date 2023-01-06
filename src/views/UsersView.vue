<template>
    <div>
        {{ $route.params.id }}
        User
    </div>
</template>

<script>
export default {
    created(){
        console.log(this.$router);
    }
}
</script>

<style scoped>

</style>