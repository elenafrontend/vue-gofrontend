<template>
  <div class="v-main-wrapper">
    <VCatalog></VCatalog>
    <VCart></VCart>
  </div>
</template>

<script>
import VCart from "./v-cart";
import VCatalog from "./v-catalog";

export default {
  name: "v-main-wrapper",
  components: {
    VCart,
    VCatalog,
  },
  props: {},
  data() {
    return {};
  },
  computed: {},
  methods: {},
  watch: {},
  mounted() {
    console.log("Hello v-main-wrapper");
  },
};
</script>

<style scoped>
.v-main-wrapper {
  max-width: 900px;
  margin: 0 auto;
}
</style>
