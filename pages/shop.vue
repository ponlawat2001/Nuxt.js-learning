<template>
  <div>
    <div v-for="product in products" :key="product.id" @click="selectedProduct = product">
      {{ product.name }} - ${{ product.price }}
    </div>
    <div v-if="selectedProduct">
      <h2>{{ selectedProduct.name }}</h2>
      <p>Price: ${{ selectedProduct.price }}</p>
      <p>Description: {{ selectedProduct.description }}</p>
      <button @click="addToCart(selectedProduct)">Add to Cart</button>
    </div>
    <div>
      <h2>Cart</h2>
      <div v-for="item in cart" :key="item.product.id">
        {{ item.product.name }} - ${{ item.product.price }} x {{ item.quantity }}
      </div>
      <div>
        Cart Total: ${{ cartTotal }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        { id: 1, name: 'Product 1', price: 10, description: 'This is a great product!' },
        { id: 2, name: 'Product 2', price: 20, description: 'This product is even better!' },
        { id: 3, name: 'Product 3', price: 30, description: 'You won\'t find a better product anywhere!' }
      ],
      selectedProduct: null,
      cart: [],
      cartTotal: 0
    }
  },
  methods: {
    addToCart(product) {
      let found = false;
      for(let i = 0; i < this.cart.length; i++) {
        if (this.cart[i].product.id === product.id) {
          this.cart[i].quantity++;
          found = true;
          break;
        }
      }
      if (!found) {
        this.cart.push({ product: product, quantity: 1 });
      }
      this.cartTotal += product.price;
    }
  }
}
</script>
