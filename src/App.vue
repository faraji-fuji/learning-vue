<script>
export default {
  // component options
  // declare some reactive state here

  data(){
    let id = 0;

    return {
      message: "Hello, World!",
      message2: "Hello Faraji, vue is awesome",
      counter: {
        count: 0
      },
      titleClass: 'title',
      count: 0,
      text: undefined,
      awesome: true,
      newTodo: '',
      todos:[
        {id: id++, text: "Learn HTML"},
        {id: id++, text: "Learn JavaScript"}
      ]
    }
  },

  methods: {
    increment(){
      // update componet state
      this.count++;
      this.counter.count++;
    },

    say_hi(){
      alert("Hi faraji");
      console.log(this.todos)
    },

    onInput(e){
      // a v-on handler recieves the native DOM event as the argument
      this.text = e.target.value
    },

    toggleAwesome(){
      this.awesome = !(this.awesome)
    },

    addTodo(e){
      let id = this.todos.length;

      let todo = {
        id: id,
        text: this.newTodo
      }


      this.todos.push(todo)
    },

    removeTodo(todo){
      this.todos.splice(todo.id, 1)
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
  <h1 v-bind:class="titleClass">{{ message }}</h1>

  <!-- Event listeners -->
  <button v-on:click="increment">count is {{ counter.count }}</button>
  <button @click="increment">count is {{ counter.count }}</button>
  <button v-on:click="say_hi">Say HI</button>

  <!-- Form bindings -->
  <form action="">
    <input  @input="onInput">
    <input v-model="text">
  </form>

  <p>{{ text }}</p>

  <!-- conditional rendering -->
  <h1 v-if="awesome">Vue is awesome!</h1>
  <h1 v-else>Oh NOoo</h1>
  <button @click="toggleAwesome">Toggle</button>

  <!-- list rendering -->
  <form @submit.prevent>
    <input v-model="newTodo">
    <button @click="addTodo">Add todo</button>

    <ul>
      <li v-for="todo in todos" :key="todo.id">
        {{ todo.text }}
        <button @click="removeTodo(todo)">X</button>
      </li>
    </ul>
    
  </form>
</template>


<style>
.title{
  color: red;
}
</style>