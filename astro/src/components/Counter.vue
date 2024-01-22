<template>
  <v-container>
    <div class="mb-4" style="height: 600px">
      <v-editor v-model="item" />
    </div>
  </v-container>
</template>

<script>
import "@bend-corp/md-editor-new/dist/VEditor/index.css";
import VEditor from "@bend-corp/md-editor-new/dist/VEditor/index.common.js";

export default {
  name: "Counter",

  components: {
    VEditor,
  },

  props: {
    ssss: {
      default: "",
    },
  },

  computed: {
    item: {
      get() {
        return this.ssss;
      },
      set(v) {
        this.$emit("input", v);
      },
    },
  },
};
</script>
