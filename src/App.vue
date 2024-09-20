<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppLinks from "./components/AppLinks.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: {
    AppHeader,
    AppMain,
    AppLinks,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppLinks />
  <AppFooter />
</template>

<style lang="scss"></style>
