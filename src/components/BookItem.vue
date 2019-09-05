<template>
  <li>{{bookItem.title}}: {{bookItem.author}}</li>
</template>

<script>
export default {
  name: "BookItem",
  props: ["bookItem"]
};
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>