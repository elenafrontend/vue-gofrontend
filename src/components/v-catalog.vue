<template>
  <div class="v-catalog">
    <h1>Catalog</h1>
    <div class="v-catalog__list">
      <VCatalogItem></VCatalogItem>
    </div>
  </div>
</template>

<script>
import VCatalogItem from './v-catalog-item'

export default {
  name: 'v-catalog',
  components: {
    VCatalogItem,
  },
  props: {},
  data() {
    return {}
  },
  computed: {},
  methods: {},
  watch: {},
  mounted() {
    console.log('Hello v-catalog');
    
  }
}
</script>

<style lang="scss">
  .v-catalog__list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
  }
</style>