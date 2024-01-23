<template>
  <nav>
    <router-link to="/">Home</router-link>
    <router-link to="/page1">Study Guide</router-link>
    <router-link to="/page2">Surprise</router-link>
  </nav>
  <div class="block">
    <h2>Study Guide</h2>


    <h3>How to learn faster</h3>
    <p>Learning is a skill that can be improved. Here are some tips to help you learn faster.</p>
    <ul>
      <li>Take notes</li>
      <li>Use flashcards</li>
      <li>Teach others</li>
      <li>Take breaks</li>
    </ul>

  </div>
</template>

<script>
export default {
  // Your component code here
  name: 'StudyGuideView',
};
</script>
