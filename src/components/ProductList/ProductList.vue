<template>
    <div>
        <h2>Products</h2>
        <template v-for="(product, index ) of products">
            <div v-bind:key={index}> 
                <h3>
                    <a>
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

import products from './products';

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
#product-list {
  padding: 0 16px;
}

.button, button {
  display: inline-flex;
  align-items: center;
  padding: 8px 16px;
  border-radius: 2px;
  font-size: 14px;
  cursor: pointer;
  background-color: #1976d2;
  color: white;
  border: none;
  margin: 4px;
}

.button:hover, button:hover {
  opacity: 0.8;
  font-weight: normal;
}

.button:disabled, button:disabled {
  opacity: 0.5;
  cursor: auto;
}

</style>
