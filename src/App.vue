<script>
export default {
  // component options
  // declare some reactive state here

  data(){
    return {
      message: "Hello, World!",
      message2: "Hello Faraji, vue is awesome",
      counter: {
        count: 0
      },
      titleClass: 'title'
    }
  }
}
</script>

<template>
  <h1 v-bind:class="titleClass">{{ message }}</h1> <!-- add a dynamic class binding here -->
  <p :class="titleClass">{{ message2 }}</p>
  <h2>Count is: {{ counter.count }}</h2>
</template>


<style>
.title{
  color: red;
}
</style>