<template>
  <section
    class="
      wrapper
      categories
      flex
      md:flex-row
      flex-col
      items-center
      justify-between
    "
  >
    <category />
    <category />
    <category />
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.categories {
  gap: 30px;
}
</style>