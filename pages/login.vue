<template>
  <div class="login">
    <div class="container">
      <div class="forms-container">
        <div class="signin-signup">
          <!-- form -->
          <form
            action=""
            class="sign-in-form"
            method="post"
            @submit.prevent="login"
          >
            <h2 class="title">Sign In</h2>
            <div class="input-field">
              <i class="fas fa-user"></i>
              <input type="email" placeholder="Your Email" v-model="email" />
            </div>
            <div class="input-field">
              <i class="fas fa-lock"></i>
              <input
                type="password"
                placeholder="Password"
                v-model="password"
              />
            </div>

            <input type="submit" value="Login" class="btn solid" />

            <p class="social-text">Or Sign in With Social platforms</p>
            <div class="social-media">
              <a href="" class="social-media">
                <a href="#" class="social-icon">
                  <i class="fab fa-facebook-f"></i>
                </a>
                <a href="#" class="social-icon">
                  <i class="fab fa-twitter"></i>
                </a>
                <a href="#" class="social-icon">
                  <i class="fab fa-google"></i>
                </a>
                <a href="#" class="social-icon">
                  <i class="fab fa-linkedin-in"></i>
                </a>
              </a>
            </div>
          </form>
          <!-- from akhir -->

          <!-- form sign up-->
          <form action="" class="sign-up-form">
            <h2 class="title">Sign up</h2>
            <div class="input-field">
              <i class="fas fa-user"></i>
              <input type="text" placeholder="Username" />
            </div>

            <div class="input-field">
              <i class="fas fa-envelope"></i>
              <input type="text" placeholder="Email" />
            </div>

            <div class="input-field">
              <i class="fas fa-lock"></i>
              <input type="password" placeholder="Password" />
            </div>
            <input type="submit" value="sign up" class="btn solid" />

            <p class="social-text">Or Sign up With Social platforms</p>
            <div class="social-media">
              <a href="" class="social-media">
                <a href="#" class="social-icon">
                  <i class="fab fa-facebook-f"></i>
                </a>
                <a href="#" class="social-icon">
                  <i class="fab fa-twitter"></i>
                </a>
                <a href="#" class="social-icon">
                  <i class="fab fa-google"></i>
                </a>
                <a href="#" class="social-icon">
                  <i class="fab fa-linkedin-in"></i>
                </a>
              </a>
            </div>
          </form>
          <!-- from akhir -->
        </div>
      </div>
      <div class="panels-container">
        <!-- pamnl 1 -->
        <div class="panel left-panel">
          <div class="content">
            <h3>Create Your Account Here</h3>
            <p>Yes, I wanna become more intelligent</p>
            <button class="btn transparent" id="sign-up-btn" @click="arrow()">
              Sign up
            </button>
          </div>
          <img src="../assets/img/rocket.svg" class="image" alt="" />
        </div>
        <!-- panel akhir -->

        <!-- pamnl 1 -->
        <div class="panel right-panel">
          <div class="content">
            <h3>One of us ?</h3>
            <p>
              Time is ticking and we are counting down the time to start learning
            </p>
            <button class="btn transparent" id="sign-in-btn" @click="remove()">
              Sign in
            </button>
          </div>
          <img src="../assets/img/desk.svg" class="image" alt="" />
        </div>
        <!-- panel akhir -->
      </div>
    </div>
  </div>
</template>
<script>
export default {
  layout: "login",
  data() {
    return {
      email: "",
      password: "",
    };
  },
  methods: {
    togglePassword() {
      var x = document.getElementById("password-content-3-5");
      if (x.type === "password") {
        x.type = "text";
        document.getElementById("icon-toggle").setAttribute("fill", "#2ec49c");
      } else {
        x.type = "password";
        document.getElementById("icon-toggle").setAttribute("fill", "#CACBCE");
      }
    },
    async login() {
      try {
        const response = await this.$auth.loginWith("local", {
          data: {
            email: this.email,
            password: this.password,
          },
        });
        // alert("Login success");
        this.$swal({
          title: "Success",
          text: `Welcome to Fullstack Academy!`,
          icon: "success",
        });
        this.$router.push("/");
      } catch (error) {
        this.$swal({
          title: "Login Failed",
          text: `Email atau Password Incorrect`,
          icon: "error",
        });
      }
    },
    arrow() {
      //   const sign_in_btn = document.querySelector("#sign-in-btn");
      //   const sign_up_btn = document.querySelector("#sign-up-btn");
      //   const containers = document.querySelector(".container");

      //   sign_up_btn.addEventListener("click", () => {
      //     containers.classList.add("sign-up-mode");
      //   });

      //   sign_in_btn.addEventListener("click", () => {
      //     containers.classList.remove("sign-up-mode");
      //   });

      const containers = document.querySelector(".container");

      containers.classList.add("sign-up-mode");
    },
    remove() {
     

      const containers = document.querySelector(".container");

      containers.classList.remove("sign-up-mode");
    },
  },
};
</script>
<style>
@import "../assets/css/login.css";
</style>