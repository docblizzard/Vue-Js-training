<template>
    <h2>Component-E</h2>
    <ComponentF></ComponentF>
</template>

<script>
import ComponentF from './ComponentF.vue';
export default {
    name: 'Component-E',
    components: {
        ComponentF,
    }
}

</script>