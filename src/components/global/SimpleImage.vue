<template functional>
  <img :src="src" :alt="alt" :height="height" :width="width"/>
</template>
<script>
export default {
  name: 'SimpleImage',
  props: {
    src: {
      type: String,
      required: true
    },
    alt: {
      type: String,
      required: true
    },
    width: {
      type: Number,
      required: true
    },
    height: {
      type: Number,
      required: true
    }
  }
}
</script>
<style lang="scss" scoped>
img {
  max-width: 100%;
  height: auto;
}
</style>
