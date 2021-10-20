<template functional>
  <img :src="src" :alt="alt" :height="height" :width="width"/>
</template>
<script>
export default {
  name: 'SimpleImage',
  props: {
    src: {
      type: String,
      require: true
    },
    alt: {
      type: String,
      require: true
    },
    width: {
      type: Number,
      require: true
    },
    height: {
      type: Number,
      require: true
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
