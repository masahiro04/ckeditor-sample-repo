<template>
  <div class="home">
    <h1>CKEditor test</h1>
    <ckeditor
      :editor="editor"
      v-model="editorData"
      :config="editorConfig"
    ></ckeditor>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import ClassicEditor from "@ckeditor/ckeditor5-build-classic";

export default defineComponent({
  name: "HomeView",
  components: {},
  setup() {
    return {
      editor: ClassicEditor,
      editorData: "<p>Content of the editor.</p>",
      editorConfig: {},
    };
  },
});
</script>
