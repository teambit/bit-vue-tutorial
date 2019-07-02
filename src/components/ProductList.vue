<template>
    <div>
        <h2>Products</h2>
        <template v-for="(product, index ) of products">
            <div v-bind:key={index}> 
                <h3>
                    <a title="product.name + ' details'">
                        {{ product.name }}
                    </a>
                </h3>
                <p v-if="product.description">
                    Description: {{ product.description }}
                </p>
                <button @click="share">
                    Share
                </button>
            </div>
        </template>
    </div>
</template>

<script>

import products from '../assets/products';

export default {
  name: 'ProductList',
  data() {
    return {products};
  },
  methods: {
      share(){
          alert('The product has been shared!')
      }
  }
}
</script>

<style>

</style>
