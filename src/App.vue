<template>
  <div id="app">
    
    <!-- Header component -->
    <TheHeader />

    <!-- Main content -->
    <main>
      <div class="bg-dark py-5">
        <div class="container">
          <p class="text-white">CONTENT GOES HERE</p>
        </div>
      </div>
    </main>

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

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter,
    BannerBlue,
    BannerSignUp
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
