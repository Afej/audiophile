<template>
  <header class="flex items-center justify-between wrapper">
    <div class="flex items-center justify-between">
      <nuxt-link to="/" class="logo mr-48 cursor-pointer">
        <img src="@/assets/images/shared/desktop/logo.svg" alt="audiophile" />
      </nuxt-link>
      
      <ul class="nav flex items-center justify-between text-white">
        <li>
          <nuxt-link to="/"> Home </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/category/headphones"> Headphones </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/category/speakers"> Speakers </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/category/earphones"> Earphones </nuxt-link>
        </li>
      </ul>
    </div>

    <div class="cart-img">
      <img src="@/assets/images/shared/desktop/icon-cart.svg" alt="cart" />
    </div>
  </header>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style lang="scss" scoped>
header {
  border-bottom: 1px solid rgba(255, 255, 255, 0.2);
  padding: 32px 0;
}

.logo {
  width: 143px;
  height: 25px;
}

.nav {
  li {
    margin-right: 34px;

    a {
      text-transform: uppercase;
      font-weight: bold;
      font-size: 13px;
      line-height: 25px;
      letter-spacing: 2px;
      transition: all 250ms ease-in-out;

      &:hover {
        color: var(--primary);
      }
    }
  }
}

.cart-img {
  width: 23.33px;
  height: 20px;
  cursor: pointer;
}
</style>