<template>
  <div>
    <!-- hero section -->
    <div class="hero bg-black">
      <main-header />

      <div class="wrapper pt-28 text-center text-white">
        <h2>
          {{ this.$route.params.type }}
        </h2>
      </div>
    </div>

    <main class="wrapper flex flex-col gap-32">
      <div
        class="
          product
          flex
          lg:flex-row
          flex-col
          items-center
          justify-between
          lg:gap-0
          gap-10
        "
      >
        <div class="product-image">
          <img
            src="@/assets/images/shared/desktop/image-xx99-mark-two-headphones.jpg"
            alt="product"
          />
        </div>

        <div class="content flex flex-col items-start">
          <p class="overline">NEW PRODUCT</p>
          <h1>XX99 Mark II Headphones</h1>
          <p class="text">
            The new XX99 Mark II headphones is the pinnacle of pristine audio.
            It redefines your premium headphone experience by reproducing the
            balanced depth and precision of studio-quality sound.
          </p>

          <button class="btn-primary">
            <nuxt-link to="/product/"> See Product </nuxt-link>
          </button>
        </div>
      </div>

      <div
        class="
          product
          flex
          lg:flex-row
          flex-col
          items-center
          justify-between
          gap-10
          lg:gap-5
        "
      >
        <div class="content flex flex-col items-start">
          <h1>XX99 Mark I Headphones</h1>
          <p class="text">
            As the gold standard for headphones, the classic XX99 Mark I offers
            detailed and accurate audio reproduction for audiophiles, mixing
            engineers, and music aficionados alike in studios and on the go.
          </p>

          <button class="btn-primary">
            <nuxt-link to="/product/"> See Product </nuxt-link>
          </button>
        </div>

        <div class="product-image">
          <img
            src="@/assets/images/shared/desktop/image-xx99-mark-one-headphones.jpg"
            alt="product"
          />
        </div>
      </div>

      <div
        class="
          product
          flex
          lg:flex-row
          flex-col
          items-center
          justify-between
          gap-10
          lg:gap-0
        "
      >
        <div class="product-image">
          <img
            src="@/assets/images/shared/desktop/image-xx59-headphones.jpg"
            alt="product"
          />
        </div>

        <div class="content flex flex-col items-start">
          <h1>
            XX59 <br />
            Headphones
          </h1>
          <p class="text">
            As the gold standard for headphones, the classic XX99 Mark I offers
            detailed and accurate audio reproduction for audiophiles, mixing
            engineers, and music aficionados alike in studios and on the go.
          </p>

          <button class="btn-primary">
            <nuxt-link to="/product/"> See Product </nuxt-link>
          </button>
        </div>
      </div>
    </main>
    <categories />
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.hero {
  height: 336px;
}

main {
  padding: 160px 0;

  @media (max-width: 768px) {
    padding: 80px 0 160px;
  }
}

.product {
  .product-image {
    width: 540px;
    height: 560px;

    @media (max-width: 768px) {
      width: 100%;
      height: 352px;
    }

    img {
      border-radius: 8px;
    }
  }

  .content {
    width: 50%;
    padding-left: 65px;

    @media (max-width: 768px) {
      width: 100%;
      text-align: center;
      align-items: center;
      padding-left: 0;
    }

    p.overline {
      margin-bottom: 24px;
      color: var(--primary);
    }

    h1 {
      margin-bottom: 32px;

      @media (max-width: 768px) {
        font-size: 28px;
        line-height: 38px;
      }
    }

    p.text {
      width: 398px;
      margin-bottom: 40px;

      @media (max-width: 768px) {
        width: 100%;
      }
    }
  }

  &:nth-of-type(2) {
    .content {
      padding-left: 0;

      @media (max-width: 768px) {
        order: 2;
      }
    }
  }
}
</style>