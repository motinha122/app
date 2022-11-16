<template>

    <div v-for="obj in todos" v-bind:key="obj.id" class="todo-list">
        <img v-bind:src="imgSrc" v-bind:alt="imgAlt" class="imagem">
        {{ obj.title }}
    </div>

</template>

<script>

export default {
    data() {
        return {
            imgSrc: 'https://64.media.tumblr.com/1940b890b307230e03c25e268fc0f75c/8b597d0c402a4868-08/s1280x1920/2261a542cf1673efcab1a5ae9e4687e0afce4d03.jpg',
            imgAlt: '1',
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
            ]
        }
    }

}

</script>

<style>
.imagem{
    width: 100px;
}

.todo-list {
    background-color: #000;
    color: #ffffff;
    margin-bottom: 5px;
}

.header {
    background: #000;
    color: aliceblue;

}
</style>