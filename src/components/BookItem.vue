<template>
  <li>{{bookItem.title}}: {{bookItem.author}}</li>
</template>

<script>
export default {
  name: "BookItem3",
  props: ["bookItem"]
};
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>