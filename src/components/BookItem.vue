<template>
  <li>{{bookItemData.title}}: {{bookItemData.author}}</li>
</template>

<script>
export default {
  name: "BookItem",
  props: ["bookItemData"]
};
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>