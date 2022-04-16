<template>
    <div>
         <section class="banner">
        <header>
            <div class="toggle"></div>
           
            
        </header>


        <div class="content">
            <h3>Final Project</h3>
            <h1>CLASSROOM</h1>
            <h3>Fullstack Developer <br> Batch 6</h3>
        </div>

        <!-- team -->
        <!-- <CardHome /> -->
          
        <!-- akhir team -->
    </section>
        
        <a href="/class">
        <div class="arrow-container animated fadeInDown">
            <div class="arrow-2">
              <i class="fa fa-angle-down"></i>
            </div>
            <div class="arrow-1 animated hinge infinite zoomIn"></div>
          </div>
        </a>

        <svg class="icons" style="display: none;">
            <symbol id="arrow-left" xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'>
              <polyline points='328 112 184 256 328 400'
                     style='fill:none;stroke:#f0f5f3;stroke-linecap:round;stroke-linejoin:round;stroke-width:48px' />
            </symbol>
            <symbol id="arrow-right" xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'>
              <polyline points='184 112 328 256 184 400'
                     style='fill:none;stroke:#f9fffd;stroke-linecap:round;stroke-linejoin:round;stroke-width:48px' />
            </symbol>
          </svg>
    </div>
</template>

<script>
export default {
    layout:'clear'
}

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700;800;900&display=swap');
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@500;600;700;800&display=swap");

/* team */
:root {
    --card-width: 250px;
    --card-height: 400px;
    --card-transition-duration: 800ms;
    --card-transition-easing: ease;
 }

 /* akhir team */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'poppins', sans-serif;
}

/* scroll */
.scroll-section {
  padding: 50px;
  
}

::-webkit-scrollbar {
  width: 0;
}

#scrollpath {
  position: fixed;
  top: 0;
  right: 0;
  width: 10px;
  height: 100%;
  
}

#progressbar {
  position: fixed;
  top: 0;
  right: 0;
  width: 10px;
  
  background: linear-gradient(to top, #008aff, #00ffe7);
  animation: anime 5s linear infinite;
}

@keyframes animate {
  0%,100% {
      filter: hue-rotate(0deg);
  }
  50% {
      filter:hue-rotate(360deg);
  }
}
#progressbar::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(to top, #008aff, #00ffe7);
  filter: blue(10px);
}
#progressbar::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(to top, #008aff, #00ffe7);
  filter: blue(30px);
}

/* scroll */
/* akhir navbar */

.banner {
    min-height: 100vh;
    background: #120e0f url(../assets/img/back-new-01.jpg);
    background-size: cover;
    background-position: center;
    padding: 26px 93px;
    display: flex;

    align-items: center;
}

header {
    position: absolute;
    top: 40px;
    display: flex;
    align-items: center;
    text-align: center;
}

.cek {
  
    width: 100px;
    height: 100px;
    margin: 0 auto;
    position: fixed;
    z-index: 99;
    top: 25px;
    left: -20%;
    right: 0;
    opacity: 0.2;
    transition: 0.5s;
}

.cek:hover {
    opacity: 1;
}

.content {
    color: white;
}

.content h3 {
    font-size: 4em;
    font-weight: 400
}

.content h1 {
    font-size: 7em;
    font-weight: 700;
    color: #D9DD26;
    
}


  button {
    border: none;
    background: none;
    cursor: pointer;
 }
  button:focus {
    outline: none;
    border: none;
 }
  

 /* akhir team */

 /* scroll */
 .arrow-container{
    width: 100px;
    height: 100px;
    margin: 0 auto;
    position: absolute;
    bottom: 25px;
    left: 0;
    right: 0;
  }
  
  .arrow-1{
    width: 100px;
    height: 100px;
    background: #00CC8E;
    opacity: 0.5;
    border-radius: 50%;
    position: absolute;
  }
  
  .arrow-2{
    width: 60px;
    height: 60px;
    background: #00CC8E;
    border-radius: 50%;
    position: absolute;
    top: 20px;
    left: 20px;
    z-index: 1;
    display: table;
  }
  
  .arrow-2:before{
    width: 52px;
    height: 52px;
    content: "";
    border: 2px solid #00CC8E;
    border-radius: 50%;
    position: absolute;
    top: 2px;
    left: 2px;
  }
  
  .arrow-2 i.fa{
    font-size: 30px;
    display: table-cell;
    vertical-align: middle;
    text-align: center;
    color: #feffff;
  }
  
  /* Custom Animate.css */
  
  .animated.hinge {
    -webkit-animation-duration: 2s;
            animation-duration: 2s;
  }
  
  @-webkit-keyframes zoomIn {
    0% {
      opacity: 0;
      -webkit-transform: scale3d(.4, .4, .4);
              transform: scale3d(.4, .4, .4);
    }
  
    50% {
      opacity: 0.5;
    }
    
    100% {
      opacity: 0;
    }
  }
  
  @keyframes zoomIn {
    0% {
      opacity: 0;
      -webkit-transform: scale3d(.4, .4, .4);
              transform: scale3d(.4, .4, .4);
    }
  
    50% {
      opacity: 0.5;
    }
    
    100% {
      opacity: 0;
    }
  }
  
  .zoomIn {
    -webkit-animation-name: zoomIn;
            animation-name: zoomIn;
  }


  /* real response */
/* @media screen and (max-width:1717px) {
  .cek {

  }
} */
@media only screen and (max-width:1440px) {
  :root {
    --card-width: 180px;
    --card-height: 400px;
 }
}

@media only screen and (max-width:1231px) {
  :root {
    --card-width: 180px;
    --card-height: 400px;
 }

 .content h1 {
   font-size: 4.5em;
 }
}

@media only screen and (max-width: 1080px) {
  .banner {
    flex-direction: column;
    text-align: center;
    align-items: center;
    justify-content: space-between;
    padding: 93px 93px 400px 93px;
    max-height: 60vh;
    
  }

  header {
    align-items: flex-start;
  }
  .content {
    align-items: center;
    justify-content: center;
  }

  .content h1 {
    font-size: 4em;
    margin: -10px;
  }

  .content h3 {
    font-size: 2em;
  }

  .info .text {
    font-size: calc(var(--card-width) * var(--text-size-offset, 0.3));
  }
  .app {
    align-items: flex-end;
    justify-content: center;
  }
  :root {
    --card-width: 151px;
    --card-height: 320px;
 }

 .arrow-container {
   width: 30px;
   height: 30px;
   
 }

 .arrow-1 {
   width: 70px;
   height: 70px;
   top: -35px;
   left: -5px;
 }

 .arrow-2 {
  width: 50px;
  height: 50px;
  
  top: -24px;
  left: 5px;
  
}

.arrow-2:before {
  width: 42px;
  height: 42px;
  
}
}

</style>