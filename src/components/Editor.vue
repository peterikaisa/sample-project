<template>
  <div>
    <div id="editor">
      <textarea :value="input" @input="update" cols="50" rows="15" />
    </div>
    <div v-html="compiled"></div>
  </div>
</template>

<script>
const marked = require("marked");

export default {
  name: "Editor",
  data() {
    return {
      input: "## Well, hello there"
    };
  },
  computed: {
    compiled() {
      return marked(this.input);
    }
  },
  methods: {
    update(e) {
      this.input = e.target.value;
    }
  }
};
</script>
