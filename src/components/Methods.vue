<template>
    <div>
        <h2> {{ name }}</h2>
        <button @click="setName">Change name</button>
        <h2> {{ count }}</h2>
        <button @click="incrementCount">Increment count</button>
        
        <h2> {{ first }} {{ last }}</h2>
        <button @click="changeHero">Change Hero</button>
    </div>
</template>

<script>
import { reactive, ref, toRefs } from 'vue';

    export default {
        name:'Methods-component',
        setup() {
            const count = ref(0)
            const state = reactive({
                first:'Bruce',
                last: 'Wayne'
            })
            function incrementCount() {
                count.value++
            }

            function changeHero(){
                state.first = 'Clark'
                state.last = 'Kent'
            }
            return {
                count,
                incrementCount,
                ...toRefs(state),
                changeHero
            }
        },
        data(){
            return{
                name:'Elwin',
            }
        },
        methods:{
            setName(){
                this.name = 'Codevolution'
            },
        },
    }
</script>

<style lang="scss" scoped>

</style>