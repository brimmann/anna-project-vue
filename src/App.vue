<template>
  <the-header />
  <RouterView />
  <the-footer/>
</template>

<script>
import TheHeader from "./components/layout/TheHeader.vue";
import TheFooter from "./components/layout/TheFooter.vue";
export default {
  components: { TheFooter, TheHeader },
};
</script>

<style>
@font-face {
  font-family: 'Opificio';
  src: url('./assets/Opificio-Light.woff2') format('woff2'),
  url('./assets/Opificio-Light.woff') format('woff');
  font-weight: 300;
  font-style: normal;
  font-display: swap;
}


body {
  background-color: white;
  font-family: 'Opificio';
  padding: 0;
  margin: 0;
}

img {
  width: 100%;
}

</style>
