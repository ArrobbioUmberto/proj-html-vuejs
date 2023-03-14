<script>
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import Specialties from './components/Specialties.vue';
import Bickford from './components/Bickford.vue';

export default {
  components: {
    Navbar,
    Hero,
    Specialties,
    Bickford

  }
}

</script>

<template>
  <header>
    <Navbar></Navbar>
    <Hero></Hero>
  </header>
  <main>
    <section class="specialities">
      <Specialties></Specialties>
      <Bickford></Bickford>
    </section>
    <section class="upcoming">
      <!-- background totale con card laterale e serie di eventi/lista sulla dx -->
    </section>
    <section class=" leader">
      <!-- una row con due col che si divino lo spazio, la prima col testo e la seconda invece con percentuali/li -->
    </section>
    <section class="latest-news">
      <!-- testo inziale con sotto card uguali ma stesso carosello hero con frecce -->
    </section>
    <section class="testimonials">
      <!-- bg nero con titolo in 'trasparenza' e sempre frecce e -->
    </section>
    <video src="">
      <!-- in questo caso immagine con pulsante play al centro, secondo step video vero -->
    </video>
    <footer>
      <section class="contact_us">
        <!-- contact us, due col che si dividono lo spazio e una col sotto con un li -->
      </section>
      <section class="">
        <!-- real footer + copyright -->
      </section>
    </footer>
  </main>
</template>

<style lang="scss" scoped>
@use './style/general.scss';

header {
  background-image: url('/img/rev-slider-main-home-img-03.jpg');
  height: 100vh;
}

.specialities {
  background-color: #fafafa;
  padding: 100px 0;
}
</style>
