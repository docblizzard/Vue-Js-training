<template>
    <!-- <button @click="getPosts">Load post</button> -->
    <div v-for="post in posts" :key="post.id">
        <h3 v-if="errorMsg">{{ errorMsg }}</h3>
        <h3>{{ post.id }} {{ post.title }}</h3>
        <p> {{ post.body }}</p>
    </div>
</template>

<script>
import axios from 'axios';
    export default {
        name: 'PostList-Component',
        created(){
            this.getPosts()
        },
        data(){
            return{
                posts: [],
                errorMsg: ''
            }
        },
        methods: {
            getPosts() {
                axios
                .get('https://jsonplaceholder.typicode.com/posts')
                .then((response) => {
                    console.log(response.data)
                    this.posts = response.data
                })
                .catch((error) =>{
                    console.log(error)
                    this.errorMsg
                })
            }
        }
    }
</script>

<style>

</style>