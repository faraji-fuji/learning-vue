<script>
    export default {
        // declare emitted events
        emits: ['response'],
        created(){
            // emit with an argument
            this.$emit('response','hello from child')
        }
    }
</script>

<template>
    <h2>Child Component</h2>
</template>