# Vue Tutorial

Learn developing with Vue. This template should help get me started
developing with Vue 3 in Vite.

## 1. Getting Started

Hello, World!

## 2. Declarative Rendering

Create a data property and use it as the text content for the `<h1>` in the 
template.

## 3. Attribute Bindings

Add a dynamic class binding to the `<h1>`, using the titleClass data property 
as its value. If it's bound correctly, the text should turn red.


## 4. Event Listeners

Implement the `increment` method and bind it to the button using `v-on`

## 5. Form Bindings

Refactor the code to use `v-model`.

## 6. Conditional Rendering

Add `v-if` and `v-else` directives to them, and implement the `toggle()` 
method so that we can use the button to toggle between them.

## 7. List Rendering

Here we have a simple todo list - try to implement the logic for `addTodo()`
and `removeTodo()` methods to make it work!

## 8.  Computed Property

Add the `filteredTodos` computed property and implement its computation 
logic! If implemented correctly, checking off a todo when hiding completed 
items should instantly hide it as well.

## 9. Lifecycle and Template Refs

Add a `mounted` hook, access the `<p>` via `this.$refs.p`, and perform some 
direct DOM operations on it (e.g. changing its `textContent`).


---

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```
