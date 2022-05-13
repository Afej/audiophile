<template>
  <div>
    <!-- hero section -->
    <div class="hero">
      <main-header />

      <div class="wrapper flex justify-center lg:justify-start">
        <div
          class="
            hero-content
            flex flex-col
            lg:items-start
            items-center
            text-white
          "
        >
          <p class="overline opacity-50">NEW PRODUCT</p>
          <h1>XX99 Mark II Headphones</h1>
          <p class="text opacity-75">
            Experience natural, lifelike audio and exceptional build quality
            made for the passionate music enthusiast.
          </p>

          <button class="btn-primary">
            <nuxt-link to="/product/"> See Product </nuxt-link>
          </button>
        </div>
      </div>
    </div>

    <main>
      <categories />

      <!-- products -->
      <section class="wrapper products flex flex-col justify-between gap-10">
        <div
          class="
            zx9
            relative
            flex
            lg:flex-row
            flex-col
            lg:justify-end
            justify-center
            items-center
            overflow-hidden
          "
        >
          <div class="patterns absolute">
            <img
              src="@/assets/images/home/desktop/pattern-circles.svg"
              alt="circles"
            />
          </div>

          <div class="zx9-img absolute -bottom-3">
            <img
              src="@/assets/images/home/desktop/image-speaker-zx9.png"
              alt="speaker zx9"
            />
          </div>

          <div class="content">
            <h1 class="mb-6 text-white">
              ZX9 <br />
              speaker
            </h1>
            <p class="opacity-75 text-white mb-10">
              Upgrade to premium speakers that are phenomenally built to deliver
              truly remarkable sound.
            </p>

            <button class="bg-black text-white">
              <nuxt-link to="/product/"> See Product </nuxt-link>
            </button>
          </div>
        </div>

        <div class="zx7 flex flex-col items-start justify-center">
          <h4 class="text-black mb-9">ZX7 speaker</h4>

          <button class="btn-secondary">
            <nuxt-link to="/product/"> See Product </nuxt-link>
          </button>
        </div>

        <div
          class="
            yx1
            flex
            md:flex-row
            flex-col
            items-center
            justify-between
            gap-10
          "
        >
          <div class="earphone-img">
            <img
              src="@/assets/images/home/desktop/image-earphones-yx1.jpg"
              alt="earphone yx1"
            />
          </div>

          <div class="content flex flex-col items-start justify-center">
            <h4 class="text-black mb-8">YX1 earphones</h4>

            <button class="btn-secondary">
              <nuxt-link to="/product/"> See Product </nuxt-link>
            </button>
          </div>
        </div>
      </section>
    </main>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
})
</script>

<style lang="scss" scoped>
.hero {
  background: url('@/assets/images/home/desktop/image-hero.jpg') no-repeat
    center center;
  height: 729px;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;

  @media (max-width: 768px) {
    background: url('@/assets/images/home/tablet/image-header.jpg') no-repeat
      center center;
    // height: 100%;
  }

  @media (max-width: 568px) {
    background: url('@/assets/images/home/mobile/image-header.jpg') no-repeat
      center center;
    // height: 100%;
  }

  &-content {
    margin-top: 128px;
    width: 398px;

    @media (max-width: 568px) {
      width: 100%;
      text-align: center;

      h1 {
        font-size: 32px;
      }

      p.text {
        width: 100% !important;
      }
    }

    p.overline {
      margin-bottom: 24px;
    }

    h1 {
      margin-bottom: 24px;
    }

    p.text {
      width: 350px;
      margin-bottom: 40px;
    }
  }
}

main {
  padding-top: 128px;
}

.products {
  padding-top: 168px;

  @media (max-width: 768px) {
    padding-top: 80px;
  }

  .zx9 {
    height: 560px;
    background: var(--primary);
    border-radius: 8px;
    padding: 0 95px 0 118px;

    @media (max-width: 768px) {
      height: 720px;
    }

    &-img {
      width: 410.23px;
      height: 493px;
      left: 118px;

      @media (max-width: 768px) {
        width: 197.21px;
        height: 237px;
        left: 35%;
        top: 52px;
      }

      @media (max-width: 568px) {
        width: 197.21px;
        height: 237px;
        left: 25%;
        top: 52px;
      }
    }

    .patterns {
      top: -60px;
      left: -150px;

      @media (max-width: 768px) {
        left: -10px;
        top: 0px;
      }
    }

    .content {
      width: 349px;

      @media (max-width: 768px) {
        margin-top: 300px;
        text-align: center;
      }

      @media (max-width: 568px) {
        width: 280px;

        h1 {
          font-size: 36px;
          line-height: 40px;
        }
      }
    }

    button {
      &:hover {
        background-color: #4c4c4c;
      }
    }
  }

  .zx7 {
    background: url('@/assets/images/home/desktop/image-speaker-zx7.jpg')
      no-repeat center center;
    height: 320px;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    padding: 0 95px;
    border-radius: 8px;

    @media (max-width: 768px) {
      padding: 0 60px;
    }

    @media (max-width: 568px) {
      padding: 0 30px;
    }
  }

  .yx1 {
    .earphone-img {
      width: 100%;
      height: 320px;
      img {
        border-radius: 8px;
      }
    }

    .content {
      padding-left: 95px;
      width: 100%;
      height: 320px;
      background-color: var(--gray-one);
      border-radius: 8px;

      @media (max-width: 768px) {
        padding-left: 30px;
      }
    }
  }
}
</style>
