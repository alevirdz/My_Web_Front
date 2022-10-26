<template>
  <div>
    <!-- ======= Contact Section ======= -->
    <section id="contact" class="contact">
      <div class="container" data-aos="fade-up">
        <div class="section-title">
          <h2>Contact</h2>
          <h3><span>Contact Us</span></h3>
          <p>
            Ut possimus qui ut temporibus culpa velit eveniet modi omnis est
            adipisci expedita at voluptas atque vitae autem.
          </p>
        </div>

        <div class="row" data-aos="fade-up" data-aos-delay="100">
          <div class="col-lg-6">
            <div class="info-box mb-4">
              <i class="fa-solid fa-location-dot"></i>
              <h3>Our Address</h3>
              <p>A108 Adam Street, New York, NY 535022</p>
            </div>
          </div>

          <div class="col-lg-3 col-md-6">
            <div class="info-box mb-4">
              <i class="fa-solid fa-envelope-open"></i>
              <h3>Email Us</h3>
              <p>contact@example.com</p>
            </div>
          </div>

          <div class="col-lg-3 col-md-6">
            <div class="info-box mb-4">
              <i class="fa-solid fa-phone"></i>
              <h3>Call Us</h3>
              <p>+1 5589 55488 55</p>
            </div>
          </div>
        </div>

        <div class="row" data-aos="fade-up" data-aos-delay="100">
          <div class="col-lg-6">
            <iframe
              class="mb-4 mb-lg-0"
              src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d12097.433213460943!2d-74.0062269!3d40.7101282!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xb89d1fe6bc499443!2sDowntown+Conference+Center!5e0!3m2!1smk!2sbg!4v1539943755621"
              frameborder="0"
              style="border: 0; width: 100%; height: 384px;"
              allowfullscreen
            ></iframe>
          </div>

          <div class="col-lg-6">
            <form
              action="forms/contact.php"
              method="post"
              role="form"
              class="php-email-form"
            >
              <div class="row">
                <div class="col form-group">
                  <input
                    type="text"
                    name="name"
                    class="form-control"
                    id="name"
                    placeholder="Nombre"
                    v-model="contact.name"
                    required
                  />
                </div>
                <div class="col form-group">
                  <input
                    type="text"
                    name="surname"
                    class="form-control"
                    id="surname"
                    placeholder="Apellido"
                    v-model="contact.surname"
                    required
                  />
                </div>
              </div>
                              <div class="col form-group">
                  <input
                    type="email"
                    class="form-control"
                    name="phone"
                    id="phone"
                    placeholder="Número telefono"
                    v-model="contact.phone"
                    required
                  />
                </div>
              <div class="form-group">
                 <input
                      type="email"
                      class="form-control"
                      name="email"
                      id="email"
                      placeholder="Correo electrónico"
                      v-model="contact.mail"
                      required
                    />
              </div>
              <div class="form-group">
                <textarea
                  class="form-control"
                  name="message"
                  rows="5"
                  placeholder="Mensaje"
                  v-model="contact.message"
                  required
                ></textarea>
              </div>
              <div class="my-3">
                <div class="loading">Loading</div>
                <div class="error-message"></div>
                <div class="sent-message">
                  Your message has been sent. Thank you!
                </div>
              </div>
              <div class="text-center">
                <button type="button" @click="sendMail">Send Message</button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </section>
    <!-- End Contact Section -->
  </div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'ContactUs',
  data() {
    return {
      contact: {},
    }
  },
  methods: {
      sendMail: function () {
      
      const objDatasContact = this.contact;
            objDatasContact.cMethod = "MethodEmail";
            console.log(objDatasContact)
        axios.post('http://localhost/Alevi/vue_web/ws_a_p_i/', objDatasContact)
      //axios.post('https://dev.crecimientoweb.com/ws_a_p_i/sendMail.php', objDatasContact)
        .then((result) => {
          console.log(result.data)
        })
        .catch(function (error) {
          console.log(error);
        });
        
    },
  },
}
</script>
<style lang="scss">
/*--------------------------------------------------------------
# Contact
--------------------------------------------------------------*/
.contact .info-box {
  color: #444444;
  text-align: center;
  box-shadow: 0 0 30px rgba(214, 215, 216, 0.3);
  padding: 20px 0 30px 0;
}
.contact .info-box i {
  font-size: 32px;
  color: #106eea;
  border-radius: 50%;
  padding: 8px;
  border: 2px dotted #b3d1fa;
}
.contact .info-box h3 {
  font-size: 20px;
  color: #777777;
  font-weight: 700;
  margin: 10px 0;
}
.contact .info-box p {
  padding: 0;
  line-height: 24px;
  font-size: 14px;
  margin-bottom: 0;
}
.contact .php-email-form {
  box-shadow: 0 0 30px rgba(214, 215, 216, 0.4);
  padding: 30px;
}
.contact .php-email-form .error-message {
  display: none;
  color: #fff;
  background: #ed3c0d;
  text-align: left;
  padding: 15px;
  font-weight: 600;
}
.contact .php-email-form .error-message br + br {
  margin-top: 25px;
}
.contact .php-email-form .sent-message {
  display: none;
  color: #fff;
  background: #18d26e;
  text-align: center;
  padding: 15px;
  font-weight: 600;
}
.contact .php-email-form .loading {
  display: none;
  background: #fff;
  text-align: center;
  padding: 15px;
}
.contact .php-email-form .loading:before {
  content: '';
  display: inline-block;
  border-radius: 50%;
  width: 24px;
  height: 24px;
  margin: 0 10px -6px 0;
  border: 3px solid #18d26e;
  border-top-color: #eee;
  -webkit-animation: animate-loading 1s linear infinite;
  animation: animate-loading 1s linear infinite;
}
.contact .php-email-form .form-group {
  margin-bottom: 20px;
}
.contact .php-email-form input,
.contact .php-email-form textarea {
  border-radius: 0;
  box-shadow: none;
  font-size: 14px;
}
.contact .php-email-form input:focus,
.contact .php-email-form textarea:focus {
  border-color: #106eea;
}
.contact .php-email-form input {
  padding: 10px 15px;
}
.contact .php-email-form textarea {
  padding: 12px 15px;
}
.contact .php-email-form button[type='submit'] {
  background: #106eea;
  border: 0;
  padding: 10px 30px;
  color: #fff;
  transition: 0.4s;
  border-radius: 4px;
}
.contact .php-email-form button[type='submit']:hover {
  background: #3b8af2;
}
@-webkit-keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
@keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
</style>
