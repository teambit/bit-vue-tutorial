<template>
  <div id="app">
    <TopBar id="top-bar"/>
    <ProductList id="product-list"/>
  </div>
</template>

<script>
import TopBar from './components/TopBar/TopBar.vue'
import ProductList from './components/ProductList/ProductList.vue'

export default {
  name: 'app',
  components: {
    TopBar, ProductList
  }
}
</script>

<style>

* {
  font-family: 'Roboto', Arial, sans-serif;
  color: #616161;
  box-sizing: border-box;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body {
  margin: 0;
}

.container {
  display: flex;
  flex-direction: row;
}

/* Text */

h1 {
  font-size: 32px;
}

h2 {
  font-size: 20px;
}

h1, h2 {
  font-weight: lighter;
}

p {
  font-size: 14px;
}

/* Hyperlink */

a {
  cursor: pointer;
  color: #1976d2;
  text-decoration: none;
}

a:hover {
  opacity: 0.8;
}

/* Input */

input {
  font-size: 14px;
  border-radius: 2px;
  padding: 8px;
  margin-bottom: 16px;
  border: 1px solid #BDBDBD;
}

label {
  font-size: 12px;
  font-weight: bold;
  margin-bottom: 4px;
  display: block;
  text-transform: uppercase;
}

/* Button */


/* Fancy Button */

.fancy-button {
  background-color: white;
  color: #1976d2;
}

.fancy-button i.material-icons {
  color: #1976d2;
  padding-right: 4px;
}

/* Top Bar */


</style>
