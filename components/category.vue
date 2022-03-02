<template>
  <div class="category flex flex-col items-center justify-end">
    <div class="category-img flex items-center">
      <img
        src="@/assets/images/shared/desktop/image-category-thumbnail-headphones.png"
        alt="category"
      />
    </div>
    <div>
      <h6>HEADPHONES</h6>

      <button class="btn-alt">
        <nuxt-link to="/"> Shop <span> > </span> </nuxt-link>
      </button>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data() {
    return {
      categories: [],
    }
  },
})
</script>

<style lang="scss" scoped>
.category {
  position: relative;
  background: var(--gray-one);
  border-radius: 8px;
  width: 100%;
  height: 204px;

  &-img {
    position: absolute;
    top: -60px;
    // left: 30%;
    width: 200px;
    height: 200px;
  }
}
</style>