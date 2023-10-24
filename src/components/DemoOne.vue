<template>
    <h2>{{ name }}</h2>
</template>

<script>
import { ref } from 'vue'
export default {
    name: 'DemoOne-component',
    setup(){
        const name = ref('Elwin')

        setTimeout(() => {
            name.value = 'Codevolution'
            console.log(name)
        }, 2000)
        return {
            name
        }
    }

}
</script>

<style lang="scss" scoped>

</style>