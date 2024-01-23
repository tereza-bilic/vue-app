<template>
  <div>
    <ul class="list">
      <li v-for="task in tasks" :key="task.id" :class="{ 'completed': task.completed }">
        {{ task.title }}
        <button @click="markAsCompleted(task.id)">X</button>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    tasks: Array
  },
  methods: {
    markAsCompleted(taskId) {
      this.$emit('mark-as-completed', taskId);
    }
  }
};
</script>

<style scoped>
.list {
  max-width: 40%;
  margin: auto;
}

.completed {
  text-decoration: line-through;
}

li {
  list-style-type: none;
  display: flex;
  justify-content: space-between;
}
</style>
