<template>
    <h2>Component-C</h2>
    <ComponentE></ComponentE>
</template>

<script>
import ComponentE from './ComponentE.vue';
export default {
    name: 'Component-C',
    components: {
        ComponentE,
    }
}

</script>