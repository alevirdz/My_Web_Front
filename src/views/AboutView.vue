<template>
  <div class="about">
    <!-- ======= Portfolio Section ======= -->
    <section id="portfolio" class="portfolio">
      <div class="container" data-aos="fade-up">
        <div class="section-title">
          <h2>Portfolio</h2>
          <h3>
            Check our
            <span>Portfolio</span>
          </h3>
          <p>
            Ut possimus qui ut temporibus culpa velit eveniet modi omnis est
            adipisci expedita at voluptas atque vitae autem.
          </p>
        </div>

        <div class="text-center">
          <vue-picture-swipe :items="items"></vue-picture-swipe>
        </div>
      </div>
    </section>
    <!-- End Portfolio Section -->
  </div>
</template>
<script>
import VuePictureSwipe from 'vue-picture-swipe'
export default {
  components: {
    VuePictureSwipe,
  },
  data() {
    return {
      items: [
        {
          src: 'https://picsum.photos/200/300',
          thumbnail: 'https://picsum.photos/200/300',
          w: 600,
          h: 400,
          alt: 'some numbers on a grey background', // optional alt attribute for thumbnail image
        },
        {
          src: 'https://picsum.photos/200/300',
          thumbnail: 'https://picsum.photos/200/300',
          w: 1200,
          h: 900,
        },
        {
          src: 'https://picsum.photos/200/300',
          thumbnail: 'https://picsum.photos/200/300',
          w: 1200,
          h: 900,
        },
        {
          src: 'https://picsum.photos/200/300',
          thumbnail: 'https://picsum.photos/200/300',
          w: 1200,
          h: 900,
        },
      ],
    }
  },
  methods: {},
  mounted() {
    console.log('Component mounted.')
  },
}
</script>
<style lang="css">
/*--------------------------------------------------------------
# Portfolio
--------------------------------------------------------------*/
.portfolio #portfolio-flters {
  padding: 0;
  margin: 0 auto 15px auto;
  list-style: none;
  text-align: center;
  border-radius: 50px;
  padding: 2px 15px;
}
.portfolio #portfolio-flters li {
  cursor: pointer;
  display: inline-block;
  padding: 10px 15px 8px 15px;
  font-size: 16px;
  font-weight: 600;
  line-height: 1;
  text-transform: uppercase;
  color: #444444;
  margin-bottom: 5px;
  transition: all 0.3s ease-in-out;
}
.portfolio #portfolio-flters li:hover,
.portfolio #portfolio-flters li.filter-active {
  color: #106eea;
}
.portfolio #portfolio-flters li:last-child {
  margin-right: 0;
}
.portfolio .portfolio-item {
  margin-bottom: 30px;
}
.portfolio .portfolio-item .portfolio-info {
  opacity: 0;
  position: absolute;
  left: 30px;
  right: 30px;
  bottom: 0;
  z-index: 3;
  transition: all ease-in-out 0.3s;
  background: rgba(255, 255, 255, 0.9);
  padding: 15px;
}
.portfolio .portfolio-item .portfolio-info h4 {
  font-size: 18px;
  color: #fff;
  font-weight: 600;
  color: #222222;
}
.portfolio .portfolio-item .portfolio-info p {
  color: #555555;
  font-size: 14px;
  margin-bottom: 0;
}
.portfolio .portfolio-item .portfolio-info .preview-link,
.portfolio .portfolio-item .portfolio-info .details-link {
  position: absolute;
  right: 40px;
  font-size: 24px;
  top: calc(50% - 18px);
  color: #3c3c3c;
}
.portfolio .portfolio-item .portfolio-info .preview-link:hover,
.portfolio .portfolio-item .portfolio-info .details-link:hover {
  color: #106eea;
}
.portfolio .portfolio-item .portfolio-info .details-link {
  right: 10px;
}
.portfolio .portfolio-item .portfolio-links {
  opacity: 0;
  left: 0;
  right: 0;
  text-align: center;
  z-index: 3;
  position: absolute;
  transition: all ease-in-out 0.3s;
}
.portfolio .portfolio-item .portfolio-links a {
  color: #fff;
  margin: 0 2px;
  font-size: 28px;
  display: inline-block;
  transition: 0.3s;
}
.portfolio .portfolio-item .portfolio-links a:hover {
  color: #6ba7f5;
}
.portfolio .portfolio-item:hover .portfolio-info {
  opacity: 1;
  bottom: 20px;
}

/*--------------------------------------------------------------
# Portfolio Details
--------------------------------------------------------------*/
.portfolio-details {
  padding-top: 40px;
}
.portfolio-details .portfolio-details-slider img {
  width: 100%;
}
.portfolio-details .portfolio-details-slider .swiper-pagination {
  margin-top: 20px;
  position: relative;
}
.portfolio-details
  .portfolio-details-slider
  .swiper-pagination
  .swiper-pagination-bullet {
  width: 12px;
  height: 12px;
  background-color: #fff;
  opacity: 1;
  border: 1px solid #106eea;
}
.portfolio-details
  .portfolio-details-slider
  .swiper-pagination
  .swiper-pagination-bullet-active {
  background-color: #106eea;
}
.portfolio-details .portfolio-info {
  padding: 30px;
  box-shadow: 0px 0 30px rgba(34, 34, 34, 0.08);
}
.portfolio-details .portfolio-info h3 {
  font-size: 22px;
  font-weight: 700;
  margin-bottom: 20px;
  padding-bottom: 20px;
  border-bottom: 1px solid #eee;
}
.portfolio-details .portfolio-info ul {
  list-style: none;
  padding: 0;
  font-size: 15px;
}
.portfolio-details .portfolio-info ul li + li {
  margin-top: 10px;
}
.portfolio-details .portfolio-description {
  padding-top: 30px;
}
.portfolio-details .portfolio-description h2 {
  font-size: 26px;
  font-weight: 700;
  margin-bottom: 20px;
}
.portfolio-details .portfolio-description p {
  padding: 0;
}
</style>
