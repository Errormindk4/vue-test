<template>
  <div class="search-field">
    <InputText placeholder="Search" />
  </div>
</template>

<script>

import InputText from "@/components/global/InputText";
export default {
  name: 'SearchFullWidth',
  components: {
    InputText
  }
}
</script>

<style lang="scss" scoped>
.search-field {
  width: 100%;
  padding: 30px 10px;
  background: $light-dark;
  border-bottom: 1px solid $dark;
}
</style>

