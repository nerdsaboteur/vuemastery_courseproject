<template>
  <div id="app">
    <NavBar />
    <NotificationContainer />
    <router-view :key="$route.fullPath" />
  </div>
</template>

<script>
import NavBar from '@/components/NavBar.vue'
import NotificationContainer from '@/components/NotificationContainer.vue'

export default {
  components: {
    NavBar,
    NotificationContainer
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.event-card {
  border: 1px solid #ccc;
  padding: 10px;
  margin: 10px;
  width: 30%;
  margin: auto;
}
.event-card a {
  text-decoration: none;
}
</style>
