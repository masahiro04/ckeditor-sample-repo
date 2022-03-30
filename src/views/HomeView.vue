<template>
  <div class="home">
    <h1>CKEditor test</h1>
    <CKEditor :editor="'ClassicEditor'" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import CKEditor from "@ckeditor/ckeditor5-vue";

export default defineComponent({
  name: "HomeView",
  components: {
    CKEditor,
  },
});
</script>
