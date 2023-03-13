<script>
import Navbar from './components/Navbar.vue';
export default {
  components: {
    Navbar
  }
}

</script>

<template>
  <header>
    <Navbar></Navbar>
  </header>
</template>

<style lang="scss" scoped>
@use './style/general.scss';

header {
  background-image: url('/img/rev-slider-main-home-img-03.jpg');
  height: 100vh;
}
</style>
