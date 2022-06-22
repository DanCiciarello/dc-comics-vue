<template>
  <div id="app">
    
    <!-- Header component -->
    <TheHeader />

    <!-- Hero image -->
    <HeroImage />

    <!-- Current Series -->
    <CardContainer />

    <!-- Banner blue with icons -->
    <BannerBlue />
    
    <!-- Footer menu -->
    <TheFooter />

    <!-- Banner with sign up CTA -->
    <BannerSignUp />
  
  </div>
</template>

<!-- ----------------------------- -->

<script>

import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";
import BannerBlue from "./components/BannerBlue.vue";
import BannerSignUp from "./components/BannerSignUp.vue";
import CardContainer from "./components/CardContainer.vue";
import HeroImage from "./components/HeroImage.vue";

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter,
    BannerBlue,
    BannerSignUp,
    CardContainer,
    HeroImage
}
}
</script>

<!-- ----------------------------- -->

<style lang="scss">

@import "./assets/scss/main.scss";

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
