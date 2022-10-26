<template>
    <div>
              <!-- ======= Services Section ======= -->
      <section id="services" class="services">
        <div class="container" data-aos="fade-up">
          <div class="section-title">
            <h2>Services</h2>
            <h3>
              Check our
              <span>Services</span>
            </h3>
            <p>
              Ut possimus qui ut temporibus culpa velit eveniet modi omnis est
              adipisci expedita at voluptas atque vitae autem.
            </p>
          </div>

          <div class="row">
            <div
              class="col-lg-4 col-md-6 d-flex align-items-stretch"
              data-aos="zoom-in"
              data-aos-delay="100"
            >
              <div class="icon-box">
                <div class="icon">
                  <i class="fa-solid fa-mobile-screen"></i>
                </div>
                <h4><a href="">Lorem Ipsum</a></h4>
                <p>
                  Voluptatum deleniti atque corrupti quos dolores et quas
                  molestias excepturi
                </p>
              </div>
            </div>

            <div
              class="col-lg-4 col-md-6 d-flex align-items-stretch mt-4 mt-md-0"
              data-aos="zoom-in"
              data-aos-delay="200"
            >
              <div class="icon-box">
                <div class="icon">
                  <i class="fa-solid fa-mobile-screen"></i>
                </div>
                <h4><a href="">Sed ut perspiciatis</a></h4>
                <p>
                  Duis aute irure dolor in reprehenderit in voluptate velit esse
                  cillum dolore
                </p>
              </div>
            </div>

            <div
              class="col-lg-4 col-md-6 d-flex align-items-stretch mt-4 mt-lg-0"
              data-aos="zoom-in"
              data-aos-delay="300"
            >
              <div class="icon-box">
                <div class="icon">
                  <i class="fa-solid fa-mobile-screen"></i>
                </div>
                <h4><a href="">Magni Dolores</a></h4>
                <p>
                  Excepteur sint occaecat cupidatat non proident, sunt in culpa
                  qui officia
                </p>
              </div>
            </div>

            <div
              class="col-lg-4 col-md-6 d-flex align-items-stretch mt-4"
              data-aos="zoom-in"
              data-aos-delay="100"
            >
              <div class="icon-box">
                <div class="icon">
                  <i class="fa-solid fa-mobile-screen"></i>
                </div>
                <h4><a href="">Nemo Enim</a></h4>
                <p>
                  At vero eos et accusamus et iusto odio dignissimos ducimus qui
                  blanditiis
                </p>
              </div>
            </div>

            <div
              class="col-lg-4 col-md-6 d-flex align-items-stretch mt-4"
              data-aos="zoom-in"
              data-aos-delay="200"
            >
              <div class="icon-box">
                <div class="icon">
                  <i class="fa-solid fa-mobile-screen"></i>
                </div>
                <h4><a href="">Dele cardo</a></h4>
                <p>
                  Quis consequatur saepe eligendi voluptatem consequatur dolor
                  consequuntur
                </p>
              </div>
            </div>

            <div
              class="col-lg-4 col-md-6 d-flex align-items-stretch mt-4"
              data-aos="zoom-in"
              data-aos-delay="300"
            >
              <div class="icon-box">
                <div class="icon">
                  <i class="fa-solid fa-mobile-screen"></i>
                </div>
                <h4><a href="">Divera don</a></h4>
                <p>
                  Modi nostrum vel laborum. Porro fugit error sit minus sapiente
                  sit aspernatur
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- End Services Section -->
    </div>
</template>

<script>
export default ({
    name: 'ServicesWeb'
})
</script>


<style lang="scss">
    /*--------------------------------------------------------------
# Services
--------------------------------------------------------------*/
.services .icon-box {
  text-align: center;
  border: 1px solid #e2eefd;
  padding: 80px 20px;
  transition: all ease-in-out 0.3s;
  background: #fff;
}
.services .icon-box .icon {
  margin: 0 auto;
  width: 64px;
  height: 64px;
  background: #f1f6fe;
  border-radius: 4px;
  border: 1px solid #deebfd;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
  transition: ease-in-out 0.3s;
}
.services .icon-box .icon i {
  color: #3b8af2;
  font-size: 28px;
  transition: ease-in-out 0.3s;
}
.services .icon-box h4 {
  font-weight: 700;
  margin-bottom: 15px;
  font-size: 24px;
}
.services .icon-box h4 a {
  color: #222222;
  transition: ease-in-out 0.3s;
}
.services .icon-box p {
  line-height: 24px;
  font-size: 14px;
  margin-bottom: 0;
}
.services .icon-box:hover {
  border-color: #fff;
  box-shadow: 0px 0 25px 0 rgba(16, 110, 234, 0.1);
}
.services .icon-box:hover h4 a,
.services .icon-box:hover .icon i {
  color: #106eea;
}
.services .icon-box:hover .icon {
  border-color: #106eea;
}
</style>