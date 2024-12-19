<template>
  <div id="app" class="bg-gray-100 min-h-screen p-6">
    <AppHeader />
    <BookList />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import BookList from './components/BookList.vue';

export default {
  components: {
    AppHeader,
    BookList,
    AppFooter,
  },
};
</script>

<style>
</style>



