<template>
    <div>
        <div>
            Form
        </div>
        <input v-model="name" type="text">
        <br>
        {{name}}
    </div>
    <div>
        <label>Carros</label><br>
        <input type="checkbox" v-model="cars" value="golf">Golf
        <input type="checkbox" v-model="cars" value="passat">Passat
        <input type="checkbox" v-model="cars" value="jetta">Jetta
        <br>
        {{cars}}
    </div>
</template>

<script>

export default {
    data() {
        return {
            name:'',
            cars:[],
        }
    }

}

</script>

<style>

</style>