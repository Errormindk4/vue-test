<template>
  <input type="text" :placeholder="placeholder" />
</template>
<script>
export default {
  name: 'InputText',
  props: {
    placeholder: {
      type: String,
      required: true
    }
  }
}
</script>
<style lang="scss" scoped>
input {
  margin: 0;
  padding: 0;
  border: none;
  width: 100%;
  background: transparent;
  outline: none;
}
</style>
