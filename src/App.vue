<script>
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import Specialties from './components/Specialties.vue';
import Bickford from './components/Bickford.vue';
import Upcoming from './components/Upcoming.vue';
import Leader from './components/Leader.vue';
import Latest_news from './components/Latest_news.vue';
import Testimonials from './components/Testimonials.vue';

export default {
  components: {
    Navbar,
    Hero,
    Specialties,
    Bickford,
    Upcoming,
    Leader,
    Latest_news,
    Testimonials
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
      <Upcoming> </Upcoming>
    </section>
    <section class=" leader">
      <Leader></Leader>
    </section>
    <section class="latest-news">
      <Latest_news></Latest_news>
    </section>
    <section class="testimonials">
      <Testimonials></Testimonials>
    </section>
    <video src="">
      <!-- in questo caso immagine con pulsante play al centro, secondo step video vero -->
    </video>
    <footer>
      <section class="contact_us">
        <!-- contact us, due col che si dividono lo spazio e una col sotto con un li -->
      </section>
      <section class="black_footer">
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

.upcoming {
  background-image: url('/img/h1-img-09.jpg');
  height: 100vh;
}

.leader {
  padding: 100px 0;
}

.latest-news {
  background-color: #fafafa;
}
</style>
