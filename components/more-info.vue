<template>
  <section
    class="
      wrapper
      more-info
      flex
      lg:flex-row
      flex-col
      items-center
      justify-between
      gap-8
    "
  >
    <div class="content lg:order-1 order-2">
      <h2 class="text-black mb-8">
        Bringing you the <br />
        <span> best </span> audio gear
      </h2>
      <p class="opacity-50">
        Located at the heart of New York City, Audiophile is the premier store
        for high end headphones, earphones, speakers, and audio accessories. We
        have a large showroom and luxury demonstration rooms available for you
        to browse and experience a wide range of our products. Stop by our store
        to meet some of the fantastic people who make Audiophile the best place
        to buy your portable audio equipment.
      </p>
    </div>
    <div class="image order-1 lg:order-2">
      <img :src="image.desktop" alt="best gear" />
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      image: {
        desktop: require('@/assets/images/shared/desktop/image-best-gear.jpg'),
        tablet: require('@/assets/images/shared/tablet/image-best-gear.jpg'),
        mobile: require('@/assets/images/shared/mobile/image-best-gear.jpg'),
      },
    }
  },
}
</script>

<style lang="scss" scoped>
.more-info {
  padding-top: 168px;
  padding-bottom: 200px;

  @media (max-width: 768px) {
    padding: 80px 0;
  }

  .content {
    width: 50%;
    // width: 445px;

    p {
      width: 445px;
    }

    h2 span {
      color: var(--primary);
    }

    @media (max-width: 1024px) {
      p {
        width: 100%;
      }
    }

    @media (max-width: 768px) {
      width: 100%;
      text-align: center;

      p {
        width: 100%;
      }
    }

    @media (max-width: 568px) {
      h2 {
        font-size: 28px;
      }
    }
  }

  .image {
    // margin-left: 125px;
    // width: 540px;
    width: 50%;
    height: 588px;

    @media (max-width: 768px) {
      width: 100%;
      height: 350px;
    }

    img {
      border-radius: 8px;
    }
  }
}
</style>