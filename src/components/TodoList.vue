<template>
  <div>
    <TodoInput 
    />
  </div>
  
</template>

<script>
import TodoInput from './TodoInput.vue';

export default {
  name: 'TodoList',
  components: {
    TodoInput,
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>