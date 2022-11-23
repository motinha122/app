<template>
    <div>
        {{fullname}}
    </div>
</template>
 
<script>

export default {
    data() {
        return {
            user:{
                firstName: 'Xamp',
                lastName: 'Son',
            }
        }
    },
    methods: {
        
    },
    computed: {
        fullname(){
            return `${this.user.firstName} ${this.user.lastName}`
        }
    }
}

</script>
 
<style>

</style>