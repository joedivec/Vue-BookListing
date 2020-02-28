<template>
<div>
  <book-form></book-form>
  <h1>{{ title }}</h1>
  <ul>
      <book-item v-for="book in books" :book='book'></book-item>
  </ul>
</div>
</template>

<script>
import BookForm from './BookForm';
import BookItem from './BookItem';

export default {
    name: 'book-list',
    components: {
      BookForm,
      BookItem
    },
    data () {
      return {
        title: 'All Books',
        books: [
            {title: 'Self-Reliance', author: 'Ralph Waldo Emerson'},
            {title: 'American Gods', author: 'Neil Gaiman'},
            {title: 'Amusing Ourselves to Death', author: 'Neil Postman'},
        ]
      }
    }
}
</script>
<style>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}
</style>
