<template>
    <div>
        <button @click="incrementCount">Clicked {{ count }} times</button>
    </div>
</template>

<script>
// import CounterMixin from '../mixins/counter.js';
import useCounter from '../composables/useCounter';
export default {
    name:'ClickCounter-component',
    // mixins: [CounterMixin],
    setup() {
        const { count, incrementCount } = useCounter(0,2)
        
        return {
            count, incrementCount
        }
    }
}
</script>

<style lang="scss" scoped>

</style>