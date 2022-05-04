<template>
  <div class="product">
    <product-cards/>
  </div>
</template>

<script>
// @ is an alias to /src
import ProductCards from '../components/ProductCards.vue'

export default {
  name: 'ProductView',
  components: {
    ProductCards
  }
}
</script>
