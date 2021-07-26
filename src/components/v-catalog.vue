<template>
  <div class="v-catalog">
    <h1>Catalog</h1>
    <VCatalogItem></VCatalogItem>
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