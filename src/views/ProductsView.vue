<template>
    <div class="container">
      <section>
        <h1>Whats in your bag</h1>
        <div class="shopping">
          <img src="https://i.postimg.cc/RZ5Jv6nG/cart.jpg" />
          <span class="quantity">0</span>
        </div>
        <button class="sortButton">Sort by Category</button>

        <select>
          <option value="all">ALL</option>
          <option value="indoor">Indoor</option>
          <option value="outdoor">Outdoor</option>
        </select>
      </section>
      <div class="list"></div>
    </div>
    <div class="card">
      <div class="check">Checkout</div>
      <h1>Shopping Cart</h1>
      <hr>
      <h2>Product Item</h2>
      <hr>
      <ul class="listCard"></ul>
      <div class="checkOut">
        <div class="total">0</div>
        <div class="closeShopping">Close</div>
      </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
    
</style>