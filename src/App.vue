<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>todo apps</h1>
    <Form :add="add"/>
    <List :todos="todos" :remove="remove" />
  </div>
</template>

<script>
import Form from './components/Form.vue'
import List from './components/List.vue'

export default {
  name: 'app',
  components: {
    Form,
    List
  },
  data() {
    return {
      todos: [],
    };
  },
  methods: {
    add(todo) {
      this.todos.push(todo);
    },
    remove(i) {
      this.todos.splice(i, 1);
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin:  0 auto;
  max-width: 1000px;
  text-align: center;
}

h1 {
  font-size: 3em;
}
</style>
