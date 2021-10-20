<template>
  <header class="container">
    <Hamburger />
    <HeaderMenu :items="items" />
    <CustomerContainer />
  </header>
</template>

<script>

import HeaderMenu from "@/components/menus/HeaderMenu";
import CustomerContainer from "@/components/common/header/CustomerContainer";
import Hamburger from "@/components/menus/Hamburger";
export default {
  name: 'Header',
  data () {
    return {
      items: [
        {url: '/', title: 'Home'},
        {url: '/', title: 'Validators'},
        {url: '/', title: 'Following'},
      ]
    }
  },
  components: {
    HeaderMenu, Hamburger, CustomerContainer
  }
}
</script>

<style lang="scss" scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  padding: 30px 0;
  height: 150px;
}
</style>

