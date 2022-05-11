<template>
  <div class="navigation">
    <div class="menuToggle" @click="toggle()"></div>
    <ul @click="list()">
      <li class="list active" style="--clr: #ffa117">
        <a href="/">
          <span class="icon"><ion-icon name="book-outline"></ion-icon></span>
          <span class="text">Classes</span>
        </a>
      </li>
      <li class="list" style="--clr: #0fc70f">
        <a href="/calendar">
          <span class="icon"
            ><ion-icon name="qr-code-outline"></ion-icon></span>
          <span class="text">Calendar</span>
        </a>
      </li>
      <!-- <li class="list" style="--clr: #2196f3">
        <a href="#">
          <span class="icon"><ion-icon name="camera-outline"></ion-icon></span>
          <span class="text">Photo</span>
        </a>
      </li> -->
      <li class="list" style="--clr: #b145e9">
        <a href="#">
          <span class="icon"
            ><ion-icon name="settings-outline"></ion-icon
          ></span>
          <span class="text">Setting</span>
        </a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  methods: {
    toggle() {
      const navigation = document.querySelector(".navigation");

      navigation.classList.toggle("open");
    },
    list() {
      const list = document.querySelectorAll(".list");
      function activeLink() {
        list.forEach((item) => item.classList.remove("active"));
        this.classList.add("active");
      }

      list.forEach((item) => {
        item.addEventListener("click", activeLink);
      });
    },
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

* {
  font-family: "Poppins", sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* body {
   
} */

.navigation {
  position: fixed;
  inset: 20px 0 20px 20px;
  width: 75px;
  background: #fff;
  z-index: 99;
  transition: 0.5s;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  top: 93px;
  left: 0;
  box-shadow: 4px 4px 5px 1px rgba(0,0,0,0.13);
-webkit-box-shadow: 4px 4px 5px 1px rgba(0,0,0,0.13);
-moz-box-shadow: 4px 4px 5px 1px rgba(0,0,0,0.13);
}

.navigation.open {
  width: 250px;
}

.navigation .menuToggle {
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

.navigation .menuToggle::before {
  content: "";
  position: absolute;
  width: 30px;
  height: 2px;
  background: #333;
  transform: translateY(-8px);
  transition: 0.5s;
}

.navigation.open .menuToggle::before {
  transform: translateY(0px) rotate(45deg);
}

.navigation .menuToggle::after {
  content: "";
  position: absolute;
  width: 30px;
  height: 2px;
  background: #333;
  transform: translateY(8px);
  transition: 0.5s;
  box-shadow: 0 -8px 0 #333;
}

.navigation.open .menuToggle::after {
  transform: translateY(0px) rotate(-45deg);
  box-shadow: 0 0 0 #333;
}

.navigation ul {
  display: flex;
  flex-direction: column;
  gap: 10px;
  width: 100%;
}

.navigation ul li {
  list-style: none;
  position: relative;
  width: 100%;
  height: 60px;
  padding: 0 10px;
  transition: 0.5s;
}
.navigation ul li.active {
    transform: translateX(30px);
}

.navigation.open ul li.active {
transform: translateX(10px);
}
.navigation ul li a {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  text-align: center;
  text-decoration: none;
}

.navigation ul li a .icon {
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

.navigation ul li.active a .icon {
  background: var(--clr);
  color: #fff;
}

.navigation ul li a .icon::before {
    content: '';
    position: absolute;
    top: 10;
    left: 0;
    width: 100%;
    height: 100%;
    background: var(--clr);
    filter: blur(8px);
    opacity: 0;
    transition: 0.5s;
}

.navigation ul li.active a .icon::before {
    opacity: 0.5;

}

.navigation ul li a .text {
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

.navigation.open ul li a .text {
    opacity: 1;
    visibility: visible;
}

.navigation ul li.active a .text {
    color: var(--clr);
}

</style>