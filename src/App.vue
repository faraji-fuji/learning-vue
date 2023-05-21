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
      }
    }
  }
}
</script>

<template>
  <h1>{{ message }}</h1>
  <p>{{ message2 }}</p>
  <h2>Count is: {{ counter.count }}</h2>
</template>
