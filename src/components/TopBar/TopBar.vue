<template>
<div>
    <a>
        <h1>My Store</h1>
    </a>
    <a class="button fancy-button"><i class="material-icons">shopping_cart</i>Checkout</a>
</div>
</template>

<style>

#top-bar {
  width: 100%;
  height: 68px;
  background-color: #1976d2;
  padding: 16px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

#top-bar h1 {
  color: white;
  margin: 0;
}

</style>

<script>
export default {
    name: 'TopBar'
}
</script>
