<script>

import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppMainLink from "./components/AppMainLinks.vue";
import AppFooter from "./components/AppFooter.vue";
import AppSignUp from "./components/AppSignUp.vue";

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
    AppSignUp
  }


};

</script>

<template>
  <div>
    <AppHeader></AppHeader>
    <AppMain></AppMain>
    <AppMainLink></AppMainLink>
    <AppFooter></AppFooter>
    <AppSignUp></AppSignUp>
  </div>
</template>

<style lang="scss" scoped></style>
