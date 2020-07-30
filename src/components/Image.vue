<template>
  <img class="Image" v-bind:src="IMAGE_BASE+image['@link']" alt="Etiam Purus" />
</template>

<script>
const IMAGE_BASE = process.env.VUE_APP_DAM_BASE_URL;

export default {
  name: "Image",
  props: ["image"],
  data() {
    return {
      imgURL: IMAGE_BASE
    };
  }
};
</script>