<script>
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import Specialties from './components/Specialties.vue';
import Bickford from './components/Bickford.vue';
import Upcoming from './components/Upcoming.vue';
import Leader from './components/Leader.vue';
import Latest_news from './components/Latest_news.vue';
import Testimonials from './components/Testimonials.vue';
import Video from './components/Video.vue';
import ContactUs from './components/ContactUs.vue';
import DarkFooter from './components/DarkFooter.vue';
import Copyright from './components/Copyright.vue';

export default {
  components: {
    Navbar,
    Hero,
    Specialties,
    Bickford,
    Upcoming,
    Leader,
    Latest_news,
    Testimonials,
    Video,
    ContactUs,
    DarkFooter,
    Copyright
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
    <section class="video">
      <Video></Video>
    </section>
  </main>
  <footer>
    <section class="contact_us">
      <ContactUs></ContactUs>
    </section>
    <section class="dark_footer">
      <DarkFooter class="darkbg"></DarkFooter>
      <Copyright class="redbg"></Copyright>
    </section>
  </footer>
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

.testimonials {
  background-color: #1e1c1c;
}

.video {
  background-image: url('/img/h1-img-04.jpg');
  height: 95vh;
  object-fit: contain;
}

.dark-footer {
  width: 100vw;
}

.darkbg {
  background-color: #181515;
}

.redbg {
  background-color: #ff4612;
}
</style>
