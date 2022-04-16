<template>
  <div>
    <div class="navigation2">
      <div class="menuToggle2" @click="toggle()"></div>
      <div class="isi-navi">
        <div class="accordion" @click="accordion()">
          <div class="contentBx active">
            <div class="label">Student</div>
            <div class="content">
              <!-- content -->
              <ul class="stat status-satu" @click="lost()">
                <li class="lost" style="--clr: #f44336">
                  <a href="#">
                    <span class="icon">
                      <img src="../../assets/img/gam1.jpg" alt="" />
                    </span>
                    <span class="text">Gilang </span>
                    <div class="navigation3" @click="navigation3()">
                      <div class="log">
                        <ion-icon name="ellipsis-vertical-outline"></ion-icon>
                      </div>
                      <ul>
                        <li>
                          <span class="icon-nav"
                            ><ion-icon name="trash-outline"></ion-icon
                          ></span>
                          <span class="text-nav"
                            ><a href="#">Hapus dari Kelas</a></span
                          >
                        </li>
                        <li>
                          <span class="icon-nav"
                            ><ion-icon
                              name="chatbubble-ellipses-outline"
                            ></ion-icon
                          ></span>
                          <span class="text-nav"
                            ><a href="#">Kirim Pesan</a></span
                          >
                        </li>
                        <li>
                          <span class="icon-nav"
                            ><ion-icon name="person-circle-outline"></ion-icon
                          ></span>
                          <span class="text-nav"
                            ><a href="#">Lihat Profile</a></span
                          >
                        </li>
                      </ul>
                    </div>
                  </a>
                </li>

                <li class="lost" style="--clr: #ffa117">
                  <a href="#">
                    <span class="icon">
                      <img src="../../assets/img/gam2.jpg" alt="" />
                    </span>
                    <span class="text">Fauzan</span>
                  </a>
                </li>
                <li class="lost" style="--clr: #0fc70f">
                  <a href="#">
                    <span class="icon">
                      <img src="../../assets/img/gam3.jpg" alt="" />
                    </span>
                    <span class="text">Aufa</span>
                  </a>
                </li>
                <li class="list" style="--clr: #2196f3">
                  <a href="#">
                    <span class="icon">
                      <img src="../../assets/img/gam4.jpg" alt="" />
                    </span>
                    <span class="text">Yhido</span>
                  </a>
                </li>

                <li class="lost" style="--clr: #b145e9">
                  <a href="#">
                    <span class="icon">
                      <img src="../../assets/img/gam5.jpg" alt="" />
                    </span>
                    <span class="text">Fransiska</span>
                  </a>
                </li>
              </ul>
              <!--  -->
              <div class="add">
                <button
                  class="btn btn-success"
                  style="border-radius: 5px"
                  data-toggle="modal"
                  data-target="#tambahKelas"
                >
                  Invite Student
                </button>
              </div>
             
            </div>
          </div>

          <div class="contentBx">
            <div class="label">Teacher</div>
            <div class="content">
              <ul class="stat status-dua">
                <li class="lost" style="--clr: #b145e9">
                  <a href="#">
                    <span class="icon">
                      <img src="../../assets/img/gam6.jpg" alt="" />
                    </span>
                    <span class="text">Ghany</span>
                  </a>
                </li>
              </ul>
              <div class="addT">
                <button
                  class="btn btn-success"
                  style="border-radius: 5px"
                  data-toggle="modal"
                  data-target="#tambahTeacher"
                >
                  Invite Teacher
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  methods: {
    toggle() {
      const navigation2 = document.querySelector(".navigation2");

      navigation2.classList.toggle("open");
    },
    accordion() {
      const accordion = document.querySelectorAll(".contentBx");
      function activeLink() {
        accordion.forEach((item) => item.classList.remove("active"));
        this.classList.add("active");
      }
      accordion.forEach((item) => {
        item.addEventListener("click", activeLink);
      });
    },

    lost() {
      const lost = document.querySelectorAll(".lost");
      function activeLink() {
        lost.forEach((item) => item.classList.remove("opened"));
        this.classList.add("opened");
      }
      lost.forEach((item) => {
        item.addEventListener("click", activeLink);
      });
    },

    navigation3() {
      const navigation3 = document.querySelector(".navigation3");

      navigation3.classList.toggle("buka");
    },
  },
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@500;600;700;800&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

.navigation2 {
  position: fixed;

  width: 75px;
  background: #fff;
  transition: 0.5s;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  padding-top: 100px;
  right: 0;
  top: 96px;
  height: 100%;
  box-shadow: 0px 5px 3px 3px rgba(0, 0, 0, 0.13);
  -webkit-box-shadow: 0px 5px 3px 3px rgba(0, 0, 0, 0.13);
  -moz-box-shadow: 0px 5px 3px 3px rgba(0, 0, 0, 0.13);
}

.navigation2.open {
  width: 250px;
}

.navigation2 .content ul li a .icon {
  left: -75px;
}

.navigation2.open .content ul li a .icon {
  left: 10px;
}
.navigation2 .menuToggle2 {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 60px;

  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  padding: 0 23px;
}

.navigation2 .menuToggle2::before {
  content: "";
  position: absolute;
  width: 30px;
  height: 2px;
  background: #333;
  transform: translateY(-8px);
  transition: 0.5s;
}

.navigation2.open .menuToggle2::before {
  transform: translateY(0px) rotate(45deg);
}

.navigation2 .menuToggle2::after {
  content: "";
  position: absolute;
  width: 30px;
  height: 2px;
  background: #333;
  transform: translateY(8px);
  transition: 0.5s;
  box-shadow: 0 -8px 0 #333;
}

.navigation2.open .menuToggle2::after {
  transform: translateY(0px) rotate(-45deg);
  box-shadow: 0 0 0 #333;
}

.navigation2 ul {
  display: flex;
  flex-direction: column;
  gap: 10px;
  width: 100%;
}

.navigation2 ul li {
  list-style: none;
  position: relative;
  width: 100%;
  height: 60px;
  padding: 0 10px;
  transition: 0.5s;
  left: 38px;
}

.navigation2.open ul li {
  left: -58px;
}

.navigation2 ul li a {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  text-align: center;
  text-decoration: none;
}

.navigation2 ul li a .icon {
  position: relative;
  display: block;
  min-width: 55px;
  height: 55px;
  line-height: 60px;
  transition: 0.5s;
  border-radius: 10px;
  font-size: 1.75em;
  color: #222;
}

.navigation2 ul li.active a .icon {
  background: var(--clr);
  color: white;
}

.navigation2 ul li a .icon::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: var(--clr);
  filter: blur(8px);
  opacity: 0;
  transition: 0.5s;
}

.navigation2 ul li.active a .icon::before {
  opacity: 0.5;
}

.navigation2 ul li a .text {
  position: relative;
  padding: 0 15px;
  height: 60px;
  display: flex;
  align-items: center;
  color: #333;
  opacity: 0;
  visibility: hidden;
  transition: 0.5s;
}

.navigation2.open ul li a {
  transform: translateX(12px);
}

.navigation2.open ul li a .text {
  opacity: 1;
  visibility: visible;
}

.navigation2 ul li.active a .text {
  color: var(--clr);
}

.navigation2 ul li.active {
  transform: translateX(-30px);
}

.navigation2.open ul li.active {
  transform: translateX(-10px);
}

.navigation2 .isi-navi {
  display: flex;
  /* justify-content: center; */
  align-items: center;
}

.accordion {
  width: 248px;
  display: flex;
}

.accordion .contentBx {
  /* position: relative; */

  display: flex;
  flex-direction: column;
}

.accordion .contentBx .label {
  position: relative;
  padding: 10px;

  color: rgb(22, 21, 21);
  cursor: pointer;
  width: 124px;

  text-align: center;
  opacity: 0;
}

.accordion .contentBx.active .label {
  font-family: "Poppins", sans-serif;
  font-weight: 600;
}

.accordion .contentBx .label:before {
  position: absolute;
  top: 50%;
  right: 20px;
  transform: translateY(-50%);
  font-size: 1.5em;
}

.accordion .contentBx .content {
  position: absolute;
  /* background: white; */
  height: 0;
  overflow: hidden;
  transition: 0.5s;
  /* overflow-y: auto; */
  top: 145px;
  left: 0px;
}

.accordion .contentBx .content .icon img {
  width: 30px;
  height: 30px;
  background-color: #008aff;
  border-radius: 20px;
  box-shadow: 1px 1px 9px 0px rgba(0, 0, 0, 0.36);
  -webkit-box-shadow: 1px 1px 9px 0px rgba(0, 0, 0, 0.36);
  -moz-box-shadow: 1px 1px 9px 0px rgba(0, 0, 0, 0.36);
}

.accordion .contentBx.active .content {
  height: 100%;
  padding: 10px;
  width: 257px;
}

.navigation2.open .accordion .label {
  opacity: 1;
}

.navigation3 {
  position: relative;
  width: 20px;
  height: 20px;
  background: rgb(255, 255, 255);
  border-radius: 10px;
  right: -70px;
}

.navigation3 ul li span {
  opacity: 0;
}
.navigation3.buka ul li span {
  opacity: 1;
}

.navigation3 ul li {
  height: 27px;
  display: flex;
  flex-direction: row;
  width: 200px;
  align-items: center;
  justify-content: flex-start;
  line-height: 2px;
  margin-left: 15px;
}
.navigation3.buka {
  position: absolute;
  width: 200px;
  height: auto;
  background: #ffffff;
  right: -40px;
  top: 30px;
  padding: 10px;
  box-shadow: -2px 2px 5px 0px rgba(0, 0, 0, 0.33);
  -webkit-box-shadow: -2px 2px 5px 0px rgba(0, 0, 0, 0.33);
  -moz-box-shadow: -2px 2px 5px 0px rgba(0, 0, 0, 0.33);
}

.navigation3.buka .log {
  position: absolute;
  left: 178px;
  top: -10px;
}
.content ul li.opened {
  z-index: 9999;
}
.content ul li .navigation3.buka ul li a {
  opacity: 1;
  text-decoration: none;
  list-style: none;
  color: black;
  z-index: 100;
  position: relative;
  line-height: -70px;
  margin-bottom: -40px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  opacity: 0.5;
}

.content ul li .navigation3.buka ul li a:hover {
  opacity: 1;
}
/* .content ul li .lost {
  display: flex;
  flex-direction: row;
} */

.navigation2 .add {
  position: relative;
  top: 250px;
  opacity: 0;
  transition: 0.5s;
}

.navigation2.open .content .add {
  position: relative;
  top: 250px;
  opacity: 1;
}

.navigation2 .addT {
  position: relative;
  top: 250px;
  opacity: 0;
  transition: 0.5s;
}

.navigation2.open .content .addT {
  position: relative;
  top: 540px;
  opacity: 1;
}
</style>
