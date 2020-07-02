<template>
  <div id="app">
   <ToDoList/>
      v-bind:todo="todo"
  </div>
</template>

<script>
  import ToDoList from "@/components/ToDoList";
export default {
  name: 'App',
    data() {
        return {
            todo: [
                {id: 1, title: 'купить хлеб', completed: false},
                {id: 2, title: 'купить пивас', completed: false},
                {id: 3, title: 'купить клей', completed: false},
            ]
        }
    },
  components: {
    ToDoList
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
