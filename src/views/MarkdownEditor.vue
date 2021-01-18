<template>
  <div>
    <h2>Editor</h2>
    <Editor />
  </div>
</template>

<script>
import Editor from "@/components/Editor.vue";

export default {
  name: "MarkdownEditor",
  components: {
    Editor
  }
};
</script>
