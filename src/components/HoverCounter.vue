<template>
    <div>
        <h2 @mouseover="incrementCount">Hovered {{ count }} times</h2>
    </div>
</template>

<script>
import useCounter from '../composables/useCounter';
export default {
    name:'HoverCounter-component',
    setup() {
        const { count, incrementCount } = useCounter(0,1)
        
        return {
            count, incrementCount
        }
    }
}
</script>

<style lang="scss" scoped>

</style>