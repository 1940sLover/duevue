<template>
  <div id="app">
    <Header theTitle = "Vue To Due"/>
    <TaskList theTitle = "My Tasks" v-bind:tasklist="tasks"/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import TaskList from './components/TaskList.vue';

export default {
  name: 'App',
  components: {
    Header,
    TaskList
  },
  data()
  {
    return {
      tasks: [
        {id: 1, title:"Learn HTML & CSS", completed: true},
        {id: 2, title:"Learn Javascript", completed: true},
        {id: 3, title:"Learn a JS Framework", completed: true}
      ]
    }
  }
}
</script>

<style>
*{
  margin: 0%;
  padding: 0%;
}
</style>
