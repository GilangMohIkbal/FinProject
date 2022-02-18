<template>
  
     <section class="h-100 w-100" style="box-sizing: border-box; background-color: #141432;width:100%; height:100%; ">
       <div class="content-2-3 container-xxl mx-auto p-0  position-relative" style="font-family: 'Poppins', sans-serif">
      <div class="text-center title-text">
        <h1 class="text-title text-white">TUGAS SANDBOX</h1>
        <p class="text-caption" style="margin-left: 3rem; margin-right: 3rem">
          Sandbox II Front-End Basic & Sandbox III Front-end Advance
        </p>
      </div>

      <div class="grid-padding text-center">
        <div class="row">
         
          <div class="col-lg-6 column">
            <div class="icon">
              <img src="http://api.elements.buildwithangga.com/storage/files/2/assets/Content/Content2/Content-2-9.png"
                alt="" />
            </div>
            <h3 class="icon-title text-white">Sandbox II <br>Front-End Basic</h3>
            <p class="icon-caption">
              input nama pembaca <br>dan judul buku kedalam list
              
            </p>
            
              <nuxt-link class="ganti" to="/sandbox2" 
              style="background-color:#707092; padding:12px 50px; border-radius:10px; color:white; margin-top:20px; text-decoration:none; display:inline-block;">
              Submit</nuxt-link>
            
            
          </div>
          <div class="col-lg-6 column">
            <div class="icon">
              <img src="http://api.elements.buildwithangga.com/storage/files/2/assets/Content/Content2/Content-2-10.png"
                alt="" />
            </div>
            <h3 class="icon-title text-white">Sandbox III <br>front-end Advance</h3>
            <p class="icon-caption">
              pengisian data dan<br />
              pemindahan data antara array/object
            </p>
            <nuxt-link class="ganti" to="/sandbox3" 
              style="background-color:#707092; padding:12px 50px; border-radius:10px; color:white; margin-top:20px; text-decoration:none; display:inline-block;">
              Submit</nuxt-link>
          </div>
        </div>
      </div>

     
    </div>
  </section> 
  
</template>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

      .content-2-3 .btn:focus,
      .content-2-3 .btn:active {
        outline: none !important;
      }

      .content-2-3 .title-text {
        padding-top: 5rem;
        margin-bottom: 3rem;
      }

      nuxt-link .ganti:hover {
        background-color: #524eee;
        
      }
      
      .content-2-3 .text-title {
        font: 600 2.25rem/2.5rem Poppins, sans-serif;
        margin-bottom: 0.625rem;
      }

      .content-2-3 .text-caption {
        color: #707092;
        font-weight: 300;
      }

      .content-2-3 .column {
        padding: 2rem 2.25rem;
      }

      .content-2-3 .icon {
        margin-bottom: 1.5rem;
      }

      .content-2-3 .icon-title {
        font: 500 1.5rem/2rem Poppins, sans-serif;
        margin-bottom: 0.625rem;
      }

      .content-2-3 .icon-caption {
        font: 400 1rem/1.625 Poppins, sans-serif;
        letter-spacing: 0.025em;
        color: #707092;
      }

      .content-2-3 .card {
        padding: 1.75rem;
        background-color: #292952;
        border-radius: 0.75rem;
        border: 1px solid #4c4c6d;
      }

      .content-2-3 .card-block {
        padding: 1rem 1rem 5rem;
      }

      .content-2-3 .card-title {
        font: 600 1.5rem/2rem Poppins, sans-serif;
        margin-bottom: 0.625rem;
      }

      .content-2-3 .card-caption {
        font: 300 1rem/1.5rem Poppins, sans-serif;
        color: #707092;
        letter-spacing: 0.025em;
        margin-bottom: 0;
      }

      .content-2-3 .btn-card {
        font: 700 1rem/1.5rem Poppins, sans-serif;
        background-color: #524eee;
        padding-top: 1rem;
        padding-bottom: 1rem;
        width: 100%;
        border-radius: 0.75rem;
        margin-bottom: 1.25rem;
        border: none;
      }

      .content-2-3 .btn-card:hover {
        --tw-shadow: inset 0 0px 25px 0 rgba(20, 20, 50, 0.7);
        box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000),
          var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
      }

      .content-2-3 .btn-outline {
        font: 400 1rem/1.5rem Poppins, sans-serif;
        color: #57578e;
        border: 1px solid #57578e;
        padding-top: 1rem;
        padding-bottom: 1rem;
        width: 100%;
        border-radius: 0.75rem;
      }

      .content-2-3 .btn-outline:hover {
        border: 1px solid #ffffff;
        color: #ffffff;
      }

      .content-2-3 .card-text {
        padding-top: 1.5rem;
        padding-bottom: 1.5rem;
      }

      .content-2-3 .grid-padding {
        padding: 0rem 1rem 3rem;
      }

      @media (min-width: 576px) {
        .content-2-3 .grid-padding {
          padding: 0rem 2rem 3rem;
        }

        .content-2-3 .card-block {
          padding: 3rem 2rem 5rem;
        }
      }

      @media (min-width: 768px) {
        .content-2-3 .grid-padding {
          padding: 0rem 4rem 3rem;
        }

        .content-2-3 .card-block {
          padding: 3rem 4rem 5rem;
        }
      }

      @media (min-width: 992px) {
        .content-2-3 .grid-padding {
          padding: 1rem 6rem 3rem;
        }

        .content-2-3 .card-block {
          padding: 3rem 6rem 5rem;
        }

        .content-2-3 .column {
          padding: 0rem 2.25rem;
        }
      }

      @media (min-width: 1200px) {
        .content-2-3 .grid-padding {
          padding: 1rem 10rem 3rem;
        }

        .content-2-3 .card-block {
          padding: 3rem 6rem 5rem;
        }

        .content-2-3 .card-btn-space {
          margin-top: 15px;
          margin-bottom: 15px;
        }

        .content-2-3 .btn-outline,
        .content-2-3 .btn-card {
          width: 95%;
          float: right;
        }
      }

      @media (max-width: 980px) {
        .content-2-3 .card-btn-space {
          width: 100%;
        }
      }
</style>


<script>
export default {
  layout:"home",
  name: 'IndexPage'
}
</script>
