<template>
  <v-previewer :value="src" />
</template>

<script>
import "@bend-corp/md-editor-new/dist/VPreviewer/index.css";
import VPreviewer from "@bend-corp/md-editor-new/dist/VPreviewer/index.common.js";
export default {
  name: "AMd",
  components: {
    VPreviewer,
  },
  props: {
    src: {
      type: String,
      default: "",
    },
  },
};
</script>
