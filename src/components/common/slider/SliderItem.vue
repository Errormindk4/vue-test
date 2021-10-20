<template>
  <div class="slide">
    <img :src="image.src" :alt="image.alt" :height="image.height" :width="image.width"/>
  </div>
</template>
<script>
export default {
  name: 'SliderItem',
  props: {
    image: {
      type: Object
    }
  }
}
</script>
<style lang="scss" scoped>
.slide {
  width: 250px;
  height: 250px;
  border: 1px solid $dark;
  border-radius: 12px;
  object-fit: cover;

  img {
    max-width: 100%;
    height: auto;
  }
}
</style>
