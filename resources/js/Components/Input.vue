<template>
    <input class="rounded-md shadow-sm border-gray-300 focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50" :value="value" @input="$emit('input', $event.target.value)" ref="input">
</template>
<script>
    export default {
        props: ['value'],
        methods: {
            focus() {
                this.$refs.input.focus()
            }
        }
    }
</script>

