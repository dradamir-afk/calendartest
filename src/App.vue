<template>
  <div id="app">
    <calendar/>
  </div>
</template>

<script>
import calendar from './components/calendar.vue'

export default {
  name: 'App',
  components: {
    calendar
  }
}
</script>

<style>
#app {
  
}
body{
  margin: 0;
}
</style>
