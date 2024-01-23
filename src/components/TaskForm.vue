<template>
  <div>
    <input v-model="newTask" />
    <button @click="addTask">Add Task</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      newTask: '',
    };
  },
  methods: {
    addTask() {
      this.$emit('add-task', this.newTask);
      this.newTask = '';
    },
  },
  emits: ['add-task'], // Declare the add-task event
};
</script>
