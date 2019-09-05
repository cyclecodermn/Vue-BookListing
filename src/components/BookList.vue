<template>
  <div>
    <h1>{{title}}</h1>
    <ul>
      <book-item3 v-for="book in books" :bookItemData="book"></book-item3>
    </ul>
    <hr />
    <book-form4 @addBook="appendBook"></book-form4>
  </div>
</template>

<script>
import BookItem3 from "./BookItem";
import BookForm4 from "./BookForm";

export default {
  name: "BookList2",
  components: {
    BookItem3,
    BookForm4
  },
  data() {
    return {
      title: "All Books2",
      books: [
        { title: "Self-Reliance", author: "Ralph Waldo Emerson" },
        { title: "American Gods", author: "Neil Gaiman" },
        { title: "Amusing Ourselves to Death", author: "Neil Postman" }
      ]
    };
  },

  methods: {
    appendBook(bookTitle, bookAuthor) {
      this.books.push({ title: bookTitle, author: bookAuthor });
    }
  }
};
</script>

<style>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
</style>