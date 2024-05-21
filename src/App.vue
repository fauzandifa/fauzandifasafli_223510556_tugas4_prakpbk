<template>
  <div id="app">
    <parent-component>
      <template #default>
        <p>tugas 4 pratikum pbk</p>
      </template>
    </parent-component>
  </div>
</template>

<script>
import ParentComponent from './components/parentcomponent.vue';

export default {
  name: 'App',
  components: {
    ParentComponent
  }
}
</script>

<style>
body {
  background-image: url('https://i.pinimg.com/564x/75/7b/db/757bdbec0b126566ea80b48948ca9906.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  margin: 0;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #f0f0f0;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

p {
  font-size: 18px;
  color: #333;
  background-color: #e0e0e0;
  padding: 10px;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
</style>
