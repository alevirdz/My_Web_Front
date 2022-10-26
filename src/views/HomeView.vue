<template>
  <div class="home">
    <Hero></Hero>
    <main id="main">
      <Feature></Feature>
      <About></About>
      <Services></Services>
      <Testimonials></Testimonials>
      <ContactUs></ContactUs>
      <Footer></Footer>
    </main>
  </div>
</template>

<script>
import Hero from '../components/sections/Hero'
import Feature from '../components/sections/FeatureServices'
import About from '../components/sections/About'
import Services from '../components/sections/Services'
import Testimonials from '../components/sections/Testimonials'
import ContactUs from '../components/sections/ContactUs'
import Footer from '../components/sections/Footer'

export default {
  name: 'HomeView',
  components: {
    Hero,
    Feature,
    About,
    Services,
    Testimonials,
    ContactUs,
    Footer,
  }
}
</script>

<style lang="scss">
/*--------------------------------------------------------------
# Sections General
--------------------------------------------------------------*/
section {
  padding: 60px 0;
  overflow: hidden;
}

.section-bg {
  background-color: #f6f9fe;
}

.section-title {
  text-align: center;
  padding-bottom: 30px;
}
.section-title h2 {
  font-size: 13px;
  letter-spacing: 1px;
  font-weight: 700;
  padding: 8px 20px;
  margin: 0;
  background: #e7f1fd;
  color: #106eea;
  display: inline-block;
  text-transform: uppercase;
  border-radius: 50px;
}
.section-title h3 {
  margin: 15px 0 0 0;
  font-size: 32px;
  font-weight: 700;
}
.section-title h3 span {
  color: #106eea;
}
.section-title p {
  margin: 15px auto 0 auto;
  font-weight: 600;
}
@media (min-width: 1024px) {
  .section-title p {
    width: 50%;
  }
}
</style>
