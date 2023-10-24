<template>
    <h2>Hello {{ name }} aka {{ heroName }}</h2>
</template>

<script>
export default {
    name:"greet-component",
    props: ['name', 'heroName']
};

</script>

