<template>
    <div>
        <input type="text" v-model="name">
    </div><br>
    {{ name }}
    <br><br>

    <input type="text" v-model="user.firstName">
    <br>
    <input type="text" v-model="user.lastName">
    <br>
    {{ user.firstName }}
    {{ user.lastName }}
    <br><br><br>

    <select v-model="pageCount">
        <option value="5">5</option>
        <option value="10">10</option>
        <option value="15">15</option>
    </select><br>
    {{ pageCount }}
</template>
 
<script>

export default {
    data() {
        return {
            name: '',
            pageCount: 5,
            user: {
                firstName: '',
                lastName: '',
            },
        }
    },
    watch: {
        name(value) {
            if (value.length >= 5) {
                this.saveUserName();
            }
        },
        pageCount() {
            this.changePage();
        },
        user: {
            handler() {
                console.log('User changed');
            },
            deep: true, //watches if any key changes in the object 
        }
    },
    methods: {
        saveUserName() {
            console.log("Saved");
            console.log(this.name);
        },
        changePage() {
            console.log("ChangePage");
        },
    },
    computed: {

    }
}

</script>
 
<style>

</style>