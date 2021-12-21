<template>
  <div class="cart-item-card">
    <h1>Cart total: ${{cart_total.toFixed(2)}}</h1>
    <button class="view-product-button">Pay by Card</button>
  </div>
</template>

<script>
export default {
  computed:{
    cart_total() {
      return this.$store.getters.cartTotal
    }
  }
}
</script>