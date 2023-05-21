<script>
export default {
    data(){
        return {
            text: ''
        }
    }
}
</script>

<template>
    <input v-model="text">

    <p>{{ text }}</p>
</template>