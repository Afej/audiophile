<template>
  <footer class="bg-black">
    <div class="wrapper flex flex-col">
      <div class="flex items-center justify-between pt-20">
        <div class="logo">
          <img src="@/assets/images/shared/desktop/logo.svg" alt="audiophile" />
        </div>
        <ul class="nav flex items-center justify-between text-white">
          <li>
            <nuxt-link to="/"> Home </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/"> Headphones </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/"> Speakers </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/"> Earphones </nuxt-link>
          </li>
        </ul>
      </div>

      <div class="flex items-end justify-between pt-9 pb-14">
        <p class="text-white opacity-50 w-5/12">
          Audiophile is an all in one stop to fulfill your audio needs. We're a
          small team of music lovers and sound specialists who are devoted to
          helping you get the most out of personal audio. Come and visit our
          demo facility - we’re open 7 days a week.
        </p>

        <ul class="flex items-center justify-between gap-4">
          <li>
            <nuxt-link to="/" class="w-6 h-6">
              <img
                src="@/assets/images/shared/desktop/icon-facebook.svg"
                alt="facebook"
              />
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" class="w-6 h-6">
              <img
                src="@/assets/images/shared/desktop/icon-twitter.svg"
                alt="twitter"
              />
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" class="w-6 h-6">
              <img
                src="@/assets/images/shared/desktop/icon-instagram.svg"
                alt="instagram"
              />
            </nuxt-link>
          </li>
        </ul>
      </div>

      <p class="text-white opacity-50 pb-12">
        Copyright 2021. All Rights Reserved
      </p>
    </div>
  </footer>
</template>

<script setup>
</script>

<style lang="scss" scoped>
.logo {
  width: 143px;
  height: 25px;
}

.nav {
  li {
    margin-right: 34px;

    &:last-child {
      margin-right: 0;
    }
    
    a {
      text-transform: uppercase;
      font-weight: bold;
      font-size: 13px;
      line-height: 25px;
      letter-spacing: 2px;
      transition: all 500ms ease-in-out;

      &:hover {
        color: var(--primary);
      }
    }
  }
}
</style>