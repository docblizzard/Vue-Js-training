<template>
    <div>
        <input type="text" :value="modelValue" @input="$emit('update:modelValue', $event.target.value)"/>
    </div>
</template>

<script>
export default {
    name: 'input-component',
    props: {
        modelValue: String
    }
}
</script>

<style scoped>
input[type='text']{
    display: block;
    width: 400px;
    padding: 6px 12px;

}

</style>