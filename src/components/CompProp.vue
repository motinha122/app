<template>
    <div>
        {{ fullname }}
    </div><br>

    <h2>Todo em Aberto</h2>
    <div v-for="todo in uncompletedTodos" :key="todo.id">
        {{todo.title}}
    </div>
    
    <h2>Todo Fechado</h2>
    <div v-for="todo in completedTodos" :key="todo.id">
        {{todo.title}}
    </div>
    
    <h2>Todos</h2>
    <div v-for="todo in todos" :key="todo.id">
        <input type="checkbox" v-model="todo.completed">
        {{todo.title}}
    </div>

</template>
 
<script>

export default {
    data() {
        return {
            user: {
                firstName: 'Xamp',
                lastName: 'Son',
            },
            todos: [
                {
                    "userId": 1,
                    "id": 1,
                    "title": "delectus aut autem",
                    "completed": false
                },
                {
                    "userId": 1,
                    "id": 2,
                    "title": "quis ut nam facilis et officia qui",
                    "completed": false
                },
                {
                    "userId": 1,
                    "id": 3,
                    "title": "fugiat veniam minus",
                    "completed": false
                },
                {
                    "userId": 1,
                    "id": 4,
                    "title": "et porro tempora",
                    "completed": true
                },
                {
                    "userId": 1,
                    "id": 5,
                    "title": "laboriosam mollitia et enim quasi adipisci quia provident illum",
                    "completed": false
                }
            ],
        }
    },
    methods: {
        
    },
    computed: {
        fullname() {
            return `${this.user.firstName} ${this.user.lastName}`;
        },
        uncompletedTodos(){
            return this.todos.filter(todo=>!todo.completed); //completed: false
        },
        completedTodos(){
            return this.todos.filter(todo=>todo.completed); //completed: true
        }
    }
}

</script>
 
<style>

</style>