<template>
  <div id="app">
    <navigation></navigation>
  </div>
</template>

<script>
import Navigation from './components/navigation/Navigation';

export default {
  name: 'app',
  components: {
    Navigation
  }
};
</script>

<style lang="scss" >
html,
body,
ul {
  margin: 0;
  padding: 0;
}
</style>
