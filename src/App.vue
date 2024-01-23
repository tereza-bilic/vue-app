<template>
  <div id="app">
    <router-view>
    </router-view>
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

a {
  color: #42b983;
}

.block {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  max-width: 40%;
  margin: auto;
}

nav {
  display: flex;
  justify-content: space-around;
  margin-bottom: 20px;
}
</style>
