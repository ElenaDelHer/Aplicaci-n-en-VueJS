<template>
  <div class="mt-8">
    <h2 class="text-2xl font-semibold mb-4">Libros de Terror</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
      <div
        v-for="book in books"
        :key="book.id"
        class="bg-white p-4 rounded-lg shadow-lg"
      >
        <h3 class="font-semibold text-lg">{{ book.title }}</h3>
        <p class="text-gray-700">{{ book.author }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BookList',
  data() {
    return {
      books: [
        { id: 1, title: "Drácula", author: "Bram Stoker" },
        { id: 2, title: "Frankenstein", author: "Mary Shelley" },
        { id: 3, title: "El Resplandor", author: "Stephen King" },
        { id: 4, title: "El Exorcista", author: "William Peter Blatty" },
      ],
    };
  },
};
</script>

<style scoped>
</style>

