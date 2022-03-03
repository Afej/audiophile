<template>
  <section class="wrapper more-info flex items-center justify-between gap-8">
    <div class="content">
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
    <div class="image">
      <img
        src="@/assets/images/shared/desktop/image-best-gear.jpg"
        alt="best gear"
      />
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.more-info {
  padding-top: 168px;
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