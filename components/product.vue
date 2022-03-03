<template>
  <div class="product text-center">
    <div class="image">
      <img
        src="@/assets/images/shared/desktop/image-xx99-mark-two-headphones.jpg"
        alt="product"
      />
    </div>

    <h5 class="text-black mt-10 mb-8">XX99 MARK II</h5>

    <button class="btn-primary">
      <nuxt-link to="/product/"> See Product </nuxt-link>
    </button>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.product {
  .image {
    height: 318px;
    width: 100%;
    // width: 350px;

    img {
      border-radius: 8px;
    }
  }
}
</style>