<template functional>
  <button>{{ caption }}</button>
</template>

<script>

export default {
  name: 'Button',
  props: {
    caption: String
  }
}
</script>

<style lang="scss" scoped>
button {
  display: flex;
  justify-content: center;
  align-items: center;
  min-width: 170px;
  height: 46px;
  border: none;
  background: #ffe600;
  font-weight: 600;
  text-transform: uppercase;
  color: #000;
  transition: all 0.5s;

  &:hover {
    color: #fff;
    background: #54440e;
  }

  &:active {
    opacity: 0.7;
  }
}
</style>
