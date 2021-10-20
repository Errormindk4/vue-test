<template>
  <div class="menu" v-if="items.length">
    <a v-for="(item, i) in items" :href="item.url" :key="i">
      {{ item.title }}
    </a>
  </div>
</template>
<script>
export default {
  name: 'HeaderMenu',
  props: {
    items: {
      type: Array,
      require: true
    }
  }
}
</script>
<style lang="scss" scoped>
.menu {
  display: flex;
  align-items: flex-start;
  justify-content: flex-end;

  a {
    font-weight: 600;
    font-size: 1.2rem;
    margin: 0 12px;
    padding-bottom: 7px;
    text-decoration: none;
    color: #fff;

    &.active, &:hover {
      border-bottom: 2px solid #000;
    }

    &:last-child {
      margin-right: 0;
    }
  }
}
</style>
