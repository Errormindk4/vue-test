<template>
  <div class="mobile-menu">
    <span/>
  </div>
</template>
<script>
export default {
  name: 'MobileMenu',
  props: {
    items: {
      type: Array,
      required: true
    }
  }
}
</script>
<style lang="scss" scoped>
.mobile-menu {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  width: 40px;
  height: 40px;

  span {
    display: block;
    height: 4px;
    background: #fff;
    width: 100%;
    position: relative;
    transition: all 0.5s;

    &:before {
      content: "";
      position: absolute;
      height: 4px;
      background: #fff;
      width: 100%;
      top: -10px;
      left: 0;
    }

    &:after {
      content: "";
      position: absolute;
      height: 4px;
      background: #fff;
      width: 60%;
      top: 12px;
      left: 0;
    }
  }
  &:hover {
    span {
      transform: rotate(45deg);

      &:before {
        transform: rotate(90deg);
        top: 0;
      }

      &:after {
        display: none;
      }
    }
  }
}
</style>
