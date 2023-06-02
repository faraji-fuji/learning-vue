<script>
export default {
    mounted(){
        // component is now mounted
        this.$refs.p.textContent = "mounted"
    }
}
</script>

<template>
  <p ref="p">hello</p>
</template>