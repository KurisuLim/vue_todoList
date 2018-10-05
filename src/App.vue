<template>
  <div id="app">
    <h1>My Todo App!</h1>
    <TodoList />
  </div>
</template>

<script>
import TodoList from './components/TodoList.vue'

export default {
  name: 'app',
  components: {
    TodoList
  }
}
</script>

<style lang="scss">
@import '../public/variables.scss/variables.scss';

*,*::before, *::after {
  box-sizing: border-box;
}
#app {
  max-width: 400px;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $vue-blue;
  margin: 0 auto;
  line-height: 1.4;
}
h1{
  text-align: center;
}
</style>
