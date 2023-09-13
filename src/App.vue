<script>
import TaskList from "./components/task-list.vue";
export default {
  name: 'App',
  components: { TaskList },
  data() {
    return {
      tasks: [
        { id: 1, title: 'Prepare Final Project Status',
          completed: false},
        { id: 2, title: 'Study Web Apps', completed: false},
        { id: 3, title: 'Do laundry', completed: false},
        { id: 4, title: 'Cook breakfast', completed: false},
        { id: 5, title: 'Learn Vue', completed: false}
      ]
    }
  }
}

</script>

<template>
  <div id="app">
    <task-list v-bind:tasks="tasks"/>
  </div>
</template>

<style scoped>

</style>
