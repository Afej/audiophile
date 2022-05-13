<template>
  <footer class="bg-black">
    <div class="relative wrapper flex flex-col">
      <div
        class="
          flex
          lg:flex-row
          flex-col
          items-center
          md:items-start
          justify-between
          lg:pt-20
          pt-14
          gap-5
          lg:gap-0
          w-full
        "
      >
        <nuxt-link to="/" class="logo cursor-pointer">
          <img src="@/assets/images/shared/desktop/logo.svg" alt="audiophile" />
        </nuxt-link>
        <ul
          class="
            nav
            flex
            md:flex-row
            flex-col
            items-center
            lg:justify-between
            text-white
            gap-4
            md:gap-0
          "
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

      <div class="flex items-end justify-between pt-9 pb-14">
        <p
          class="
            text-white
            opacity-50
            lg:w-5/12
            w-full
            text-center
            md:text-left
          "
        >
          Audiophile is an all in one stop to fulfill your audio needs. We're a
          small team of music lovers and sound specialists who are devoted to
          helping you get the most out of personal audio. Come and visit our
          demo facility - we’re open 7 days a week.
        </p>

        <ul class="lg:flex hidden items-center justify-between gap-4">
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

      <div class="flex md:flex-row flex-col justify-between items-center pb-12">
        <p class="text-white opacity-50 md:pb-0 pb-10">
          Copyright 2021. All Rights Reserved
        </p>

        <ul class="lg:hidden flex items-center gap-4">
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
    </div>
  </footer>
</template>

<script setup>
</script>

<style lang="scss" scoped>
.wrapper::after {
  content: '';
  position: absolute;
  top: 0;
  width: 101px;
  height: 4px;
  background: var(--primary);
}

.logo {
  width: 143px;
  height: 25px;
}

.nav {
  li {
    margin-right: 34px;

    @media (max-width: 568px) {
      margin-right: 0;
    }

    &:last-child {
      margin-right: 0;
    }

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
</style>