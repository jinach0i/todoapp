<template>
  <div id="app">
    <TodoHeader></TodoHeader>
    <TodoInput></TodoInput>
    <TodoList></TodoList>
    <TodoFooter></TodoFooter>
  </div>
</template>
<script>
export default{
  components: {
    'TodoHeader' : TodoHeader,
    'TodoInput' : TodoInput,
    'TodoList' : TodoList,
    'TodoFooter' : TodoFooter,
  }
}
import TodoHeader from './components/TodoHeader.vue'
import TodoInput from './components/TodoInput.vue'
import TodoList from './components/TodoList.vue'
import TodoFooter from './components/TodoFooter.vue'
</script>
<style>
  body{text-align: center; box-sizing: border-box; margin: 0 auto; padding: 0;}
  input{width: 200px; border: 1px groove green;}
  button{border: 1px double black;}
  div.shadow{box-shadow: 5px 10px 10px rgba(0, 0, 0, .03);}
</style>