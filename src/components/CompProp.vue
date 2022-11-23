<template>
    <div>
        {{ fullname }}
    </div>
    <div v-for="todo in todos" :key="todo.id">
        {{todo.title}}
        <span>{{todo.completed}}</span>
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
            return `${this.user.firstName} ${this.user.lastName}`
        },
        uncompletedTodos(){
            return this.todos
        }
    }
}

</script>
 
<style>

</style>