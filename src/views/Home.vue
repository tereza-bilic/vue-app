<template>
  <div>
    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/page1">Study Guide</router-link>
      <router-link to="/page2">Surprise</router-link>
    </nav>
    <h1>Task Management App</h1>
    <TaskForm @add-task="addTask" />
    <TaskList :tasks="tasks" @mark-as-completed="markAsCompleted" />
    <p>Total Tasks: {{ tasks.length }}</p>
    <p>Completed Tasks: {{ completedTasksCount }}</p>
  </div>
</template>

<script>
import TaskForm from '@/components/TaskForm.vue';
import TaskList from '@/components/TaskList.vue';

export default {
  name: 'HomeView',
  components: {
    TaskForm,
    TaskList
  },
  data() {
    return {
      tasks: [
        { id: 1, title: 'Complete Vue project', completed: false },
        { id: 2, title: 'Study for exam', completed: true },
        { id: 3, title: 'Buy groceries', completed: false },
        { id: 4, title: 'Pay bills', completed: false}
      ],
    };
  },
  computed: {
    completedTasksCount() {
      return this.tasks.filter(task => task.completed).length;
    },
  },
  methods: {
    addTask(newTask) {
      const taskId = this.tasks.length + 1;
      this.tasks.push({ id: taskId, title: newTask, completed: false });
    },
    markAsCompleted(taskId) {
      const taskIndex = this.tasks.findIndex(task => task.id === taskId);
      if (taskIndex !== -1) {
        this.tasks[taskIndex].completed = true;
      }
    },
  },
};
</script>

<style scoped>
/* Your scoped styles here */
</style>
