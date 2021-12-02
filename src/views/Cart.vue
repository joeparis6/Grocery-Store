<template>
<div>
  <h1>Your Cart</h1>
  <ProductList :products="cart" />
</div>
<footer>
  <a href="https://github.com/BYUCS260/grocery-store-joeparis6">https://github.com/BYUCS260/grocery-store-joeparis6</a>
</footer>
</template>

<script>
import ProductList from "../components/ProductList.vue"
export default {
  name: 'Browse',
  components: {
    ProductList
  },
  data() {
    return {

    }
  },
  computed: {
    cart() {
      return this.$root.$data.cart;
    }
  },

}
</script>
