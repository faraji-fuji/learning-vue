<!-- declarative rendering -->
<script>
export default {
    data(){
        return {
            counter:{
                count: 0
            },
            message: "Hello Faraji"
        }
    }
}
</script>

<template>
    <h2>{{ message }}</h2>
    <p>Count is: {{ counter.count }}</p>
</template>

