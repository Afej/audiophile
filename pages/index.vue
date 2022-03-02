<template>
  <div>
    <!-- hero section -->
    <div class="hero text-white">
      <main-header />

      <div class="wrapper">
        <div class="hero-content flex flex-col items-start justify-start">
          <p class="overline">NEW PRODUCT</p>
          <h1>XX99 Mark II Headphones</h1>
          <p class="text">
            Experience natural, lifelike audio and exceptional build quality
            made for the passionate music enthusiast.
          </p>

          <button class="btn-primary">See Product</button>
        </div>
      </div>
    </div>

    <section class="wrapper flex items-center justify-between categories">
      <category />
      <category />
      <category />
    </section>

    <section class="wrapper products flex flex-col justify-between gap-10">
      <div class="zx9 relative flex justify-end items-center overflow-hidden">
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

          <button class="bg-black text-white">See product</button>
        </div>
      </div>

      <div class="zx7 flex flex-col items-start justify-center">
        <h4 class="text-black mb-9">ZX7 speaker</h4>

        <button class="btn-secondary">See product</button>
      </div>

      <div class="yx1 flex items-center justify-between gap-10">
        <div class="earphone-img">
          <img
            src="@/assets/images/home/desktop/image-earphones-yx1.jpg"
            alt="earphone yx1"
          />
        </div>

        <div class="content flex flex-col items-start justify-center">
          <h4 class="text-black mb-8">YX1 earphones</h4>

          <button class="btn-secondary">See product</button>
        </div>
      </div>
    </section>

    <section class="wrapper more-info flex items-center justify-between gap-8">
      <div class="content">
        <h2 class="text-black mb-8">
          Bringing you the <br />
          <span> best </span> audio gear
        </h2>
        <p class="opacity-50">
          Located at the heart of New York City, Audiophile is the premier store
          for high end headphones, earphones, speakers, and audio accessories.
          We have a large showroom and luxury demonstration rooms available for
          you to browse and experience a wide range of our products. Stop by our
          store to meet some of the fantastic people who make Audiophile the
          best place to buy your portable audio equipment.
        </p>
      </div>
      <div class="image">
        <img
          src="@/assets/images/shared/desktop/image-best-gear.jpg"
          alt="best gear"
        />
      </div>
    </section>

    <main-footer />
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

  &-content {
    margin-top: 128px;
    width: 398px;

    p.overline {
      margin-bottom: 24px;
    }

    h1 {
      margin-bottom: 24px;
    }

    p.text {
      margin-bottom: 40px;
    }
  }
}

.categories {
  gap: 30px;
  padding-top: 128px;
  padding-bottom: 168px;
}

.products {
  padding-bottom: 168px;

  .zx9 {
    height: 560px;
    background: var(--primary);
    border-radius: 8px;
    padding: 0 95px 0 118px;

    &-img {
      width: 410.23px;
      height: 493px;
      left: 118px;
    }

    .patterns {
      top: -60px;
      left: -150px;
    }

    .content {
      width: 349px;
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
    }
  }
}

.more-info {
  padding-bottom: 200px;
  .content {
    width: 50%;
    // width: 445px;

    p {
      width: 445px;
    }

    h2 span {
      color: var(--primary);
    }
  }

  .image {
    // margin-left: 125px;
    width: 50%;
    // width: 540px;
    height: 588px;

    img {
      border-radius: 8px;
    }
  }
}
</style>
