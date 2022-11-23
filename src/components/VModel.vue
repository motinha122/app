<template>

    <div>
        <label>Nome</label><br>
        <input v-model="name" type="text"><br>
        {{ name }}
        <br>
    </div>

    <div>
        <label>Sports</label><br>
        <select v-model="sports">
            <option value="">Escolha</option>
            <option value="futebol">Futebol</option>
            <option value="skate">Skate</option>
            <option value="tenis">tenis</option>
        </select>
        {{sports}}
        <br>
    </div>

    <div>
        <label>Newsletter</label><br>
        <input type="radio" v-model="newsletter" value="Sim">Sim
        <input type="radio" v-model="newsletter" value="Não">Não<br>
        {{newsletter}}
    </div>


</template>

<script>

export default {
    data() {
        return {
            name:"Xampson",
            sports:'Xampson',
            newsletter:'Sim'
        }
    }
}

</script>

<style>

</style>