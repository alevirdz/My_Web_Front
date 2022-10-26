<template>
    <div>
            <section id="hero" class="d-flex align-items-center">
      <div class="container" data-aos="zoom-out" data-aos-delay="100">
        <h1>
          Welcome to
          <span>BizLand</span>
        </h1>
        <h2>
          We are team of talented designers making websites with Bootstrap
        </h2>
        <div class="d-flex">
          <a href="#about" class="btn-get-started scrollto">Get Started</a>
          <!-- <a
            href="https://www.youtube.com/watch?v=O6MFjchcQX0"
            class="glightbox btn-watch-video"
          >
            <i class="bi bi-play-circle"></i>
            <span>Watch Video</span>
          </a> -->

          <CoolLightBox
            :items="items"
            :index="index"
            @close="index = null"
          ></CoolLightBox>
          <div class="images-wrapper">
            <div
              class="image"
              v-for="(image, imageIndex) in items"
              :key="imageIndex"
              @click="index = imageIndex"
              :style="{ backgroundImage: 'url(' + image.src + ')' }"
            ></div>
          </div>
        </div>
      </div>
    </section>
    <!-- End Hero -->
    </div>
</template>
<script>
import { CoolLightBox } from 'vue-cool-lightbox'
export default {
    name: 'HeroWeb',
    components:{
        CoolLightBox,
    }
}
</script>
<style lang="scss">
    /*--------------------------------------------------------------
# Hero Section
--------------------------------------------------------------*/
#hero {
  width: 100%;
  height: 75vh;
  background: url('https://picsum.photos/200/300') top left;
  background-size: cover;
  position: relative;
}
#hero:before {
  content: '';
  background: rgba(255, 255, 255, 0.6);
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
}
#hero .container {
  position: relative;
}
#hero h1 {
  margin: 0;
  font-size: 48px;
  font-weight: 700;
  line-height: 56px;
  color: #222222;
  font-family: 'Poppins', sans-serif;
}
#hero h1 span {
  color: #106eea;
}
#hero h2 {
  color: #555555;
  margin: 5px 0 30px 0;
  font-size: 24px;
  font-weight: 400;
}
#hero .btn-get-started {
  font-family: 'Roboto', sans-serif;
  text-transform: uppercase;
  font-weight: 500;
  font-size: 14px;
  letter-spacing: 1px;
  display: inline-block;
  padding: 10px 28px;
  border-radius: 4px;
  transition: 0.5s;
  color: #fff;
  background: #106eea;
}
#hero .btn-get-started:hover {
  background: #247cf0;
}
#hero .btn-watch-video {
  font-size: 16px;
  transition: 0.5s;
  margin-left: 25px;
  color: #222222;
  font-weight: 600;
  display: flex;
  align-items: center;
}
#hero .btn-watch-video i {
  color: #106eea;
  font-size: 32px;
  transition: 0.3s;
  line-height: 0;
  margin-right: 8px;
}
#hero .btn-watch-video:hover {
  color: #106eea;
}
#hero .btn-watch-video:hover i {
  color: #3b8af2;
}
@media (min-width: 1024px) {
  #hero {
    background-attachment: fixed;
  }
}
@media (max-width: 768px) {
  #hero {
    height: 100vh;
  }
  #hero h1 {
    font-size: 28px;
    line-height: 36px;
  }
  #hero h2 {
    font-size: 18px;
    line-height: 24px;
    margin-bottom: 30px;
  }
  #hero .btn-get-started,
  #hero .btn-watch-video {
    font-size: 13px;
  }
}
@media (max-height: 500px) {
  #hero {
    height: 120vh;
  }
}

</style>