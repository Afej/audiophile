<template>
  <header
    class="
      flex
      md:items-center
      items-start
      justify-between
      wrapper
      md:py-8
      py-6
    "
  >
    <div class="md:flex md:items-center justify-between">
      <div class="flex justify-between items-center gap-11">
        <div class="md:hidden icon text-2xl text-white duration-500">
          <i
            :class="[open ? 'fa-solid fa-xmark' : 'fa-solid fa-bars']"
            @click="toggleNav"
          ></i>
        </div>
        <nuxt-link to="/" class="logo mr-48 cursor-pointer">
          <img src="@/assets/images/shared/desktop/logo.svg" alt="audiophile" />
        </nuxt-link>
      </div>

      <ul
        class="
          nav
          md:flex md:items-center
          justify-between
          text-white
          md:py-0
          py-10
          md:w-auto
          w-full
          md:static
          absolute
          top-14
          duration-700
          ease-in
        "
        :class="[open ? 'left-12' : '-left-full']"
      >
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


<script>
export default {
  data() {
    return {
      open: true,
    }
  },
  methods: {
    toggleNav() {
      this.open = !this.open
    },
  },
}
</script>


<style lang="scss" scoped>
header {
  border-bottom: 1px solid rgba(255, 255, 255, 0.2);
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