<template>
  <div class="container1">
    <!-- banner -->
    <div class="header"></div>
    <!-- title -->
    <div class="title">
      <div class="judul">
        <p>Daftar Kelas</p>
      </div>
      <div class="menu">
        <div class="tambah">
          <button class="btn btn-secondary" style="border-radius: 5px" data-toggle="modal" data-target="#tambahKelas">
            Tambah Kelas
          </button>
        </div>
        <div class="join">
          <button class="btn btn-success" style="border-radius: 5px" data-toggle="modal" data-target="#joinKelas">
            Join Kelas
          </button>
        </div>
      </div>
    </div>
    <div class="content">
      <Cards />
    </div>
<!-- Modal u/ Tambah kelas -->
<div class="modal fade" id="tambahKelas" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered">
    <div class="modal-content">
      
        <Form />
      
    </div>
  </div>
</div>

<!-- Modal u/ Join Kelas -->
<div class="modal fade" id="joinKelas" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      
        <Join />
      
    </div>
  </div>
</div>


  </div>
</template>


<script>
export default {
  layout: "classpage",
};
</script>
<style scoped>
@import "../assets/css/class.css"
</style>