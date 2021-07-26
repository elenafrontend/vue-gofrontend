<template>
  <div class="v-catalog-item">
    <img
      class="v-catalog-item__image"
      :src="require('../assets/images/' + product_data.image)"
      alt=""
    />
    <h2 class="v-catalog-item__name">{{ product_data.name }}</h2>
    <p class="v-catalog-item__price">Price: {{ product_data.price }} p.</p>
    <button class="v-catalog-item__btn btn" @click="sendData">
      Add to cart
    </button>
  </div>
</template>

<script>
export default {
  name: "v-catalog-item",
  components: {},
  props: {
    product_data: {
      type: Object,
      default() {
        return {};
      },
    },
  },
  data() {
    return {};
  },
  computed: {},
  methods: {
    sendData() {
      this.$emit("sendArticle", this.product_data.article);
    },
  },
};
</script>

<style lang="scss">
.v-catalog-item {
  flex-basis: 25%;
  box-shadow: 0 0 8px 0 #e0e0e0;
  margin-bottom: $margin * 3;
  padding: $padding * 2;
}
.v-catalog-item__image {
  max-height: 300px;
}
</style>
