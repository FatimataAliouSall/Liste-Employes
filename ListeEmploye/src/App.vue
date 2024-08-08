<template>
  <div id="app">
    <EmployesList />
  </div>
</template>

<script>
import EmployesList from './components/EmployesList.vue'

export default {
  name: 'App',
  components: {
    EmployesList
  }
}
</script>

<style>
@import './assets/style.css';
</style>
