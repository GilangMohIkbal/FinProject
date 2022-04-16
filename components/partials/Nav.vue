<template>
    <div>
         <section class="h-100 w-00 bg-white" style="box-sizing: border-box"></section>
        <nav class="navbar-1-2 navbar navbar-expand-lg navbar-light p-4 px-md-4 mb-3 bg-body"
      style="font-family: Poppins, sans-serif">
      <div class="container">
        <a class="navbar-brand" href="#">
          
          <h4 style="color: rgb(115, 116, 117);">Fullstack Developer</h4>
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02"
          aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link px-md-4 active" aria-current="page" href="#"></a>
            </li>
            <li class="nav-item">
              <a class="nav-link px-md-4" href="#"></a>
            </li>
            <li class="nav-item">
              <a class="nav-link px-md-4" href="#"></a>
            </li>
            <li class="nav-item">
              <a class="nav-link px-md-4" href="#"></a>
            </li>
            <li class="nav-item">
              <a class="nav-link px-md-4" href="#"></a>
            </li>
          </ul>
          <div class="d-flex">
            <a href="#" class="dropdown-item has-icon  log" style="border-radius: 20px; padding: 10px 25px; transition: 0.5s;" @click="logout">
                <i class="fas fa-sign-out-alt"></i> Logout
              </a>
          </div>
        </div>
      </div>
    </nav>
    </div>
</template>
<script>
export default {
    methods: {
    async logout() {
      await this.$auth.logout();
      await this.$router.push("/login");
      this.$swal({
            title: "Success",
            text: `Anda Berhasil Logout`,
            icon: "success",
          });
    },
  },
}
</script>

<style>
.navbar-1-2.navbar-light .navbar-nav .nav-link {
  color: #092a33;
  transition: 0.3s;
}

nav {
    box-shadow: 0px 1px 3px 3px rgba(0,0,0,0.13);
-webkit-box-shadow: 0px 1px 3px 3px rgba(0,0,0,0.13);
-moz-box-shadow: 0px 1px 3px 3px rgba(0,0,0,0.13);
}

.navbar-1-2.navbar-light .navbar-nav .nav-link.active {
  font-weight: 500;
}

.navbar-1-2 .btn-get-started {
  border-radius: 20px;
  padding: 12px 30px;
  font-weight: 500;
}

.navbar-1-2 .btn-get-started-yellow {
  background-color: #ffdda9;
  color: #372642;
  transition: 0.3s;
}

.navbar-1-2 .btn-get-started-yellow:hover {
  background-color: #fcd396;
  color: #372642;
  transition: 0.3s;
}

.d-flex a:hover {
    background-color: #fd3838;
    color: white;
}
</style>