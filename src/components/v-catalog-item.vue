<template>
  <div class="v-catalog-item">
    <h2>Item 1</h2>
    <p>Price: 100</p>
    <button>Add to cart</button>
  </div>
</template>

<script>

export default {
  name: 'v-main-item',
  components: {},
  props: {},
  data() {
    return {}
  },
  computed: {},
  methods: {},
  watch: {},
  mounted() {
    console.log('Hello v-catalog-item');
    
  }
}
</script>

<style lang="scss">
  .v-catalog-item {
    flex-basis: 25%;
    box-shadow: 0 0 8px 0 #e0e0e0;
    margin-bottom: $margin * 2;
    padding: $padding * 2;
  }
</style>