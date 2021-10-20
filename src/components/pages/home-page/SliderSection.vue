<template>
  <div class="slider">
    <h2>{{ title }}</h2>
    <div class="slides">
      <SliderItem v-for="(item, i) in items" :key="i" :title="item.title" :image="item.image" />
    </div>
  </div>
</template>

<script>

import SliderItem from "@/components/common/slider/SliderItem";
export default {
  name: 'SliderSection',
  components: {SliderItem},
  props: {
    items: {
      type: Array,
      required: true
    },
    title: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.slider {
  margin: 25px 0;

  h2 {
    font-size: 3.5rem;
    margin: 25px 0;
    font-weight: 800;
    color: $dark;
  }

  .slides {
    display: flex;

    > div {
      margin: 10px;
    }
  }
}
</style>

