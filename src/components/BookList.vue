<template>
<div>
  <h1>{{ title }}
</div>
</template>

<script>
export default {
    name: 'book-list',
    data () {
      return {
        title: 'All Books'
      }
    }
}
</script>
<style>
h1, h2 {
  font-weight: normal;
}
</style>
