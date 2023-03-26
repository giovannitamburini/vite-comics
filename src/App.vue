<script>

import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppMainLink from "./components/AppMainLinks.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  data() {
    return {

    };
  },

  components: {
    AppHeader,
    AppMain,
    AppMainLink,
    AppFooter,
  }


};

</script>

<template>
  <div>
    <AppHeader></AppHeader>
    <AppMain></AppMain>
    <AppMainLink></AppMainLink>
    <AppFooter></AppFooter>
  </div>
</template>

<style lang="scss" scoped></style>
