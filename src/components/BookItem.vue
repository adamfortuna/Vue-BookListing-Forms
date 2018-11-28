<template>
  <li>
    {{book.title}} : {{book.author}}
    <span class="is--read" v-if="book.finishedReading">Read</span>
    <span class="is--not-read"v-else="book.finishedReading">Not Read</span>

  </li>
</template>

<script>
export default {
  name: 'BookItem',
  props: ['book'],
};
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
.is--read {
  color: green;
}
.is--not-read {
  color: red;
}
</style>
