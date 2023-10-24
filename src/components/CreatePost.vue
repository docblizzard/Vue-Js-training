<template>
    <div>
        <form @submit.prevent="createPost">
            <div>
                <label for="userId">Post user id</label>
                <input type="text" id="userId" v-model="FormData.userId">
            </div>
            <div>
                <label for="title">Post title</label>
                <input type="text" id="title" v-model="FormData.title">
            </div>
            <div>
                <label for="body">Post body</label>
                <input type="text" id="body" v-model="FormData.body">
            </div>
        <button>Create Post</button>
        </form>
    </div>
</template>

<script>
import axios from 'axios';
    export default {
        name: 'CreatePost-component',
        data(){
            return {
                FormData: {
                    userId: '',
                    title:'',
                    body:'',
                }
            }
        },
        methods: {
            createPost(){
                axios.post('https://jsonplaceholder.typicode.com/posts', this.formData)
                .then(response => console.log(response))
                .catch(error => console.log(error))
            }
        }
    }
</script>

<style>

</style>