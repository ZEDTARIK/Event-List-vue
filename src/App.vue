<template>
  <nav id="app">
    <router-link to="/">Events</router-link> |
    <router-link to="/about">About</router-link>
  </nav>

  <h4>Good Events</h4>
  
  <router-view />
</template>

<script>
export default {
  name: "App",
}
</script>
<style>
#app {
  text-align: center;
  padding: 30px;
}
h4 {
  font-size: 20px;
}
</style>
