<template>
    <div>
              <!-- ======= About Section ======= -->
      <section id="about" class="about section-bg">
        <div class="container" data-aos="fade-up">
          <div class="section-title">
            <h2>About</h2>
            <h3>
              Find Out More
              <span>About Us</span>
            </h3>
            <p>
              Ut possimus qui ut temporibus culpa velit eveniet modi omnis est
              adipisci expedita at voluptas atque vitae autem.
            </p>
          </div>

          <div class="row">
            <div class="col-lg-6" data-aos="fade-right" data-aos-delay="100">
              <img
                src="https://picsum.photos/800/800"
                class="img-fluid"
                alt=""
              />
            </div>
            <div
              class="col-lg-6 pt-4 pt-lg-0 content d-flex flex-column justify-content-center"
              data-aos="fade-up"
              data-aos-delay="100"
            >
              <h3>
                Voluptatem dignissimos provident quasi corporis voluptates sit
                assumenda.
              </h3>
              <p class="fst-italic">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </p>
              <ul>
                <li>
                  <i class="bx bx-store-alt"></i>
                  <div>
                    <h5>Ullamco laboris nisi ut aliquip consequat</h5>
                    <p>
                      Magni facilis facilis repellendus cum excepturi quaerat
                      praesentium libre trade
                    </p>
                  </div>
                </li>
                <li>
                  <i class="bx bx-images"></i>
                  <div>
                    <h5>Magnam soluta odio exercitationem reprehenderi</h5>
                    <p>
                      Quo totam dolorum at pariatur aut distinctio dolorum
                      laudantium illo direna pasata redi
                    </p>
                  </div>
                </li>
              </ul>
              <p>
                Ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis
                aute irure dolor in reprehenderit in voluptate velit esse cillum
                dolore eu fugiat nulla pariatur. Excepteur sint occaecat
                cupidatat non proident, sunt in culpa qui officia deserunt
                mollit anim id est laborum
              </p>
            </div>
          </div>
        </div>
      </section>
      <!-- End About Section -->
    </div>
</template>

<script>
export default {
    name: 'AboutWeb'
}
</script>
<style lang="scss">
    /*--------------------------------------------------------------
# About
--------------------------------------------------------------*/
.about .content h3 {
  font-weight: 600;
  font-size: 26px;
}
.about .content ul {
  list-style: none;
  padding: 0;
}
.about .content ul li {
  display: flex;
  align-items: flex-start;
  margin-bottom: 35px;
}
.about .content ul li:first-child {
  margin-top: 35px;
}
.about .content ul i {
  background: #fff;
  box-shadow: 0px 6px 15px rgba(16, 110, 234, 0.12);
  font-size: 24px;
  padding: 20px;
  margin-right: 15px;
  color: #106eea;
  border-radius: 50px;
}
.about .content ul h5 {
  font-size: 18px;
  color: #555555;
}
.about .content ul p {
  font-size: 15px;
}
.about .content p:last-child {
  margin-bottom: 0;
}

</style>