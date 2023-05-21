<!-- Attribute bindings -->
<script>
export default{
    data(){
        return{
            titleClass: 'title'
        }
    }
}
</script>

<template>
    <h2 :class="titleClass">Make me Red</h2>
</template>

<style>
.title{
    color: red;
}
</style>