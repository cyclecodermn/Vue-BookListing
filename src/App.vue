<template>
  <div id="app">
    <img src="./assets/logo.png">
    <book-list2></book-list2>
  </div>
</template>

<script>
import BookList2 from './components/BookList';

export default {
  name: 'app',
  components: {
    BookList2,
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
