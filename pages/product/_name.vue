<template>
  <div>
    <!-- hero section -->
    <div class="hero bg-black text-white">
      <main-header />
    </div>

    <div class="wrapper flex flex-col justify-start pt-20 pb-60">
      <nuxt-link to="/" class="back-btn text-black opacity-50 cursor-pointer">
        Go Back
      </nuxt-link>

      <main class="flex flex-col justify-start gap-32 pt-14">
        <div class="product flex items-center justify-between">
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

            <h6 class="text-black mb-12">$ 2,999</h6>

            <div class="flex items-center gap-4">
              <button
                class="cart-btn text-black flex items-center justify-between"
              >
                <span> - </span> 1 <span> + </span>
              </button>
              <button class="btn-primary">
                Add to cart
                <!-- <nuxt-link to="/checkout"> ADD TO CART </nuxt-link> -->
              </button>
            </div>
          </div>
        </div>

        <div class="features flex items-start justify-between gap-10">
          <div class="content">
            <h3 class="mb-8">FEATURES</h3>
            <p class="opacity-50">
              Featuring a genuine leather head strap and premium earcups, these
              headphones deliver superior comfort for those who like to enjoy
              endless listening. It includes intuitive controls designed for any
              situation. Whether you’re taking a business call or just in your
              own personal space, the auto on/off and pause features ensure that
              you’ll never miss a beat.
            </p>
            <br />
            <br />
            <p class="opacity-50">
              The advanced Active Noise Cancellation with built-in equalizer
              allow you to experience your audio world on your terms. It lets
              you enjoy your audio in peace, but quickly interact with your
              surroundings when you need to. Combined with Bluetooth 5. 0
              compliant connectivity and 17 hour battery life, the XX99 Mark II
              headphones gives you superior sound, cutting-edge technology, and
              a modern design aesthetic.
            </p>
          </div>
          <div class="box-items">
            <h3 class="mb-8">in the box</h3>

            <p class="box-item text-black">
              <span> 1x </span>
              Headphone Unit
            </p>
            <p class="box-item text-black">
              <span> 1x </span>
              Headphone Unit
            </p>
            <p class="box-item text-black">
              <span> 1x </span>
              Headphone Unit
            </p>
            <p class="box-item text-black">
              <span> 1x </span>
              Headphone Unit
            </p>
            <p class="box-item text-black">
              <span> 1x </span>
              Headphone Unit
            </p>
          </div>
        </div>

        <div class="product-images flex justify-between gap-10">
          <div class="flex flex-col justify-between w-2/5">
            <div class="img-1">
              <img
                src="@/assets/images/product-xx99-mark-two-headphones/desktop/image-gallery-1.jpg"
                alt=""
              />
            </div>
            <div class="img-2">
              <img
                src="@/assets/images/product-xx99-mark-two-headphones/desktop/image-gallery-2.jpg"
                alt=""
              />
            </div>
          </div>

          <div class="img-3">
            <img
              src="@/assets/images/product-xx99-mark-two-headphones/desktop/image-gallery-3.jpg"
              alt=""
            />
          </div>
        </div>

        <div class="other-products">
          <h3 class="text-black text-center mb-16">you may also like</h3>

          <div class="products flex items-center justify-between gap-0">
            <product />
            <product />
            <product />
          </div>
        </div>
      </main>
    </div>
    <categories />
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
// main {
// }

.back-btn {
  width: 60px;

  &:hover {
    color: var(--primary);
    opacity: 1;
  }
}

.product {
  .product-image {
    width: 540px;
    height: 560px;
    border-radius: 8px;

    img {
      border-radius: 8px;
    }
  }

  .content {
    width: 50%;
    padding-left: 65px;

    p.overline {
      margin-bottom: 16px;
      color: var(--primary);
    }

    h1 {
      margin-bottom: 32px;
    }

    p.text {
      width: 398px;
      margin-bottom: 32px;
    }

    .cart-btn {
      background-color: var(--gray-one);
      width: 120px;
      padding: 15px 16px;

      span {
        opacity: 0.25;

        &:hover {
          color: var(--primary);
          opacity: 1;
        }
      }
    }
  }
}

.features {
  .content {
    width: 635px;
  }

  .box-items {
    width: 350px;

    .box-item {
      margin-bottom: 10px;
      //   opacity: 0.5;

      span {
        color: var(--primary);
        opacity: 1 !important;
        margin-right: 24px;
      }
    }
  }
}

.product-images {
  img {
    border-radius: 8px;
  }

  .img-1,
  .img-2 {
    width: 100%;
    height: 280px;
  }

  .img-3 {
    height: 592px;
    width: 635px;
  }
}
</style>