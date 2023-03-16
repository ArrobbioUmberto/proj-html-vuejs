<script>
import Navbar from './components/header/Navbar.vue';
import Hero from './components/header/Hero.vue';
import Specialties from './components/main/Specialties.vue';
import Bickford from './components/main/Bickford.vue';
import Upcoming from './components/main/Upcoming.vue';
import Leader from './components/main/Leader.vue';
import Latest_news from './components/main/Latest_news.vue';
import Testimonials from './components/main/Testimonials.vue';
import Video from './components/main/Video.vue';
import ContactUs from './components/footer/ContactUs.vue';
import DarkFooter from './components/footer/DarkFooter.vue';
import Copyright from './components/footer/Copyright.vue';

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
    <section class="footer">
      <DarkFooter></DarkFooter>
    </section>
    <Copyright class="redbg"></Copyright>
  </footer>
</template>

<style lang="scss" scoped>
@use './style/general.scss';

header {
  background-image: url('/img/rev-slider-main-home-img-03.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
}

.specialities {
  background-color: #fafafa;
  padding: 100px 0;
}

.upcoming {
  background-image: url('/img/h1-img-09.jpg');
  background-repeat: no-repeat;
  background-size: cover;
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
  background-repeat: no-repeat;
  background-size: cover;
  height: 95vh;
}

.footer {
  background-color: #181515;
}

.redbg {
  background-color: #ff4612;
  margin-top: -16px;
}
</style>
