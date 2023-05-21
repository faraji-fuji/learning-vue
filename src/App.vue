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
      titleClass: 'title',
      count: 0
    }
  },

  methods: {
    increment(){
      // update componet state
      this.count++;
      this.counter.count++;
    },

    say_hi(){
      alert("Hi faraji")
    }
  }
}
</script>

<template>
  <!-- Declarative rendering -->
  <h1>{{ message }}</h1>
  <h2>Count is: {{ counter.count }}</h2>

  <!-- Attribute binding  -->
  <p :class="titleClass">{{ message2 }}</p>
  <h1 v-bind:class="titleClass">{{ message }}</h1> <!-- add a dynamic class binding here -->


  <!-- Event listeners -->
  <button v-on:click="increment">count is {{ counter.count }}</button>
  <button @click="increment">count is {{ counter.count }}</button>
  <button v-on:click="say_hi">Say HI</button>
</template>


<style>
.title{
  color: red;
}
</style>