<template>
  <nav>
    <router-link to="/">Home</router-link>
    <router-link to="/page1">Study Guide</router-link>
    <router-link to="/page2">Surprise</router-link>
  </nav>
  <div>
    <h2>Hi</h2>
    <!-- Your content here -->
    <img src="../assets/cat.webp" alt="cat" width="500">
  </div>
</template>

<script>
export default {
  // Your component code here
  name: 'Page2View',
};
</script>
