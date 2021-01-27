<template>
  <div class="home container-fluid m-0 p-0">
    <div id="home-page" class="bg-danger p-4 full-height">
      <div class="container pt-3">
        <div class="row pb-5">
          <div class="col-lg-6 col-md-12 pt-4 m-auto text-center">
            <img
              id="iphone-img"
              src="../assets/travelTreasuryiPhone.png"
              alt=""
            />
          </div>
          <div class="col-lg-6 col-md-12 my-auto pt-4">
            <div class="text-center mb-3">
              <h1 class="display-3">
                {{ title }}
                <h3>Find The World</h3>
              </h1>
            </div>
            <div
              class="border p-3 bg-white rounded shadow p-md-5 p-3 text-center"
            >
              <h2>Coming soon</h2>
              <form action="">
                <div class="form-group">
                  <label for="email"
                    >Reserve your account now, we'll contact you when it's
                    live</label
                  >
                  <input
                    type="text"
                    id="email"
                    placeholder="Enter Email"
                    class="form-control"
                    v-model="email"
                  />
                  <small id="emailHelp" class="form-text text-muted"
                    >We'll never share your email address</small
                  >
                  <button type="submit" class="btn btn-success mt-3">
                    Join Waiting List
                  </button>
                  <div class="mt-4">
                    <p class="m-0">{{ message }}</p>
                  </div>
                </div>
              </form>
            </div>
            <div class="available p-2">
              <h4 class="text-center mb-4 mt-3 text-light">Available on</h4>
              <div class="row">
                <div class="col my-auto">
                  <img
                    src="../assets/download_apple.png"
                    alt=""
                    class="img-fluid app_store_img float-right"
                  />
                </div>
                <div class="col my-auto">
                  <img
                    src="../assets/download_google.png"
                    class="img-fluid app_store_img float-left"
                    alt=""
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="about" class="bg-warning p-4 full-height bg-light p-3 p-md-5">
      <div class="row">
        <div class="col-lg-4 text-center">
          <!-- icon made by freepik -->
          <img src="../assets/icons/app.svg" height="120" class="m-4" alt="" />
          <h5 class="ml-md-4 mr-md-4">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fuga ex
            fugiat ut, et consectetur deleniti cumque. Assumenda rem cumque enim
            nostrum accusantium voluptatem tempora, nesciunt debitis et
            quibusdam optio temporibus?
          </h5>
        </div>
        <div class="col-lg-4 text-center">
          <!-- icon made by freepik -->
          <img
            src="../assets/icons/piggy-bank.svg"
            height="120"
            class="m-4"
            alt=""
          />
          <h5 class="ml-md-4 mr-md-4">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fuga ex
            fugiat ut, et consectetur deleniti cumque. Assumenda rem cumque enim
            nostrum accusantium voluptatem tempora, nesciunt debitis et
            quibusdam optio temporibus?
          </h5>
        </div>
        <div class="col-lg-4 text-center">
          <!-- icon made by freepik -->
          <img
            src="../assets/icons/passport.svg"
            height="120"
            class="m-4"
            alt=""
          />
          <h5 class="ml-md-4 mr-md-4">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fuga ex
            fugiat ut, et consectetur deleniti cumque. Assumenda rem cumque enim
            nostrum accusantium voluptatem tempora, nesciunt debitis et
            quibusdam optio temporibus?
          </h5>
        </div>
      </div>
    </div>
    <div id="contact" class="p-4 full-height">
      <div class="row justify-content-center my-3">
        <div class="col-lg-4 text-center">
          <h2>Have Any Questions?</h2>
          <p>Contact us by filling put the information below</p>

          <form action="">
            <div class="form-group text-left">
              <input
                type="email"
                name=""
                class="form-control"
                placeholder="Enter your email"
                id="email"
              />
              <textarea
                class="form-control mt-3"
                placeholder="Enter your message"
                rows="5"
              ></textarea>
            </div>
            <button type="submit" class="btn btn-primary">Send Message</button>
          </form>
        </div>
      </div>
    </div>
    <div id="footer" class="p-4 full-height">
      <footer class="text-light p-4">
        <a href="" class="text-warning">Build This App</a> |
        <a href="" class="text-warning">Privacy Policy</a>
        <br />
        <small>&copy; 2020, TravelTreasury.app</small>
      </footer>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  data() {
    return {
      title: "Travel Treasury",
    };
  },
};
</script>

<style scoped>
.full-height {
  min-height: 580px;
}
#home-page {
  background-color: ;
  background: url("../assets/bg_mt.jpg") no-repeat center center;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -moz-background-size: cover;
  background-size: cover;
}

#iphone-img {
  max-height: 500px;
}

.app_store_img {
  max-height: 80px;
}

#about {
  min-width: 40px;
  min-height: 200px;
}
#contact {
  min-height: 400px;
  background: rgb(98, 123, 236);
  color: white;
}

#footer {
  min-height: 100px;
  display: flex;
  justify-content: center;
  text-align: center;
  color: white;
  background: rgb(53, 51, 51);
}
</style>