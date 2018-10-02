<template>
  <div class="app">
    <TodoList></TodoList>
  </div>
</template>

<script>
import TodoList from './components/TodoList';

export default {
  name: 'App',
  components: {
    TodoList,
  },
  data() {
    return {
      todo: [{
        title: 'To water flowers',
        project: 'House',
        done: false,
      }, {
        title: 'Pay the bills',
        project: 'House',
        done: true,
      }, {
        title: 'Buy products',
        project: 'Family',
        done: false,
      }, {
        title: 'Meet parents',
        project: 'Family',
        done: false,
      }],
    };
  },
};
</script>

<style>
.app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
