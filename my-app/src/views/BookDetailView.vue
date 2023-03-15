<template>
  <div>This is C view</div>
  <Book />
</template>
<script lang="ts">
import { defineComponent } from "vue";
import Book from "@/components/BookFront.vue";
export default defineComponent({
  components: { Book },
});
</script>
<style scoped></style>
