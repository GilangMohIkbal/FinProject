<template>
  <div class="isi-materi">
    <!-- list materi -->
    <div class="list-materi">
      <div class="title"><p>List Tugas</p></div>
      <div class="title-list" id="progressbar">
        <div class="scroll-bar">
          <!--  -->
          <div
            class="nav flex-column nav-pills"
            id="v-pills-tab"
            role="tablist"
            aria-orientation="vertical"
          >
          <h5>Javanscript Basic</h5>
          
            <a
              class="nav-link"
              id="v-pills-pengantar-tab"
              data-toggle="pill"
              href="#v-pills-pengantar"
              role="tab"
              aria-controls="v-pills-pengantar"
              aria-selected="true"
              >SANDBOX</a
            >
              
          </div>
         
          <!-- akhir list -->
        </div>
      </div>
    </div>
    <!-- akhir list materi -->

    <!-- isi content -->
    <div class="content-isi-materi">
      <div class="tab-content" id="v-pills-tabContent">
        <div
          class="tab-pane fade show active"
          id="v-pills-pengantar"
          role="tabpanel"
          aria-labelledby="v-pills-home-tab"
        >
          <h3>Tugas SandBox</h3>
          <p>
            Buatlah TodoList Perpustakaan
          </p>
        </div>
      </div>

     
    </div>
    <!-- akhir isi content -->
  </div>
</template>

<style scoped>
.list-materi {
  background-color: rgb(255, 255, 255);
  height: 600px;
  min-width: 300px;
  border-radius: 20px;

  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  padding: 10px;
}
.list-materi {
  background-color: rgb(255, 255, 255);
  height: 600px;
  min-width: 300px;
  border-radius: 20px;

  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  padding: 10px;
}

.list-materi title {
  justify-content: center;
  align-items: flex-start;
  text-align: center;
  display: flex;
  height: 30%;
  width: 100%;
  font-size: 40px;
}

.list-materi .title-list {
  justify-content: flex-start;
  height: 70%;
  width: 100%;
}

.list-materi .title-list ul {
  padding-left: 0rem;
}
.list-materi .title-list ul li {
  list-style: none;
  margin: 10px 0;
  text-align: center;
  padding: 0px 5px;
}

.list-materi .title-list ul li a {
  color: black;
  text-decoration: none;
  background-color: rgb(208, 225, 239);
  padding: 5px 30px;
  width: 100%;
  display: flex;
  justify-content: stretch;
  align-items: center;
  border-radius: 10px;
}

.list-materi .title-list ul li a:hover {
  background-color: rgb(190, 216, 236);
  margin-top: 5px;
  margin-bottom: -5px;
  box-shadow: 12px 11px 5px -10px rgba(0, 0, 0, 0.19);
  -webkit-box-shadow: 12px 11px 5px -10px rgba(0, 0, 0, 0.19);
  -moz-box-shadow: 12px 11px 5px -10px rgba(0, 0, 0, 0.19);
}
::-webkit-scrollbar {
  width: 0;
}

.scroll-bar {
  height: 500px;
  width: 100%;
  scroll-behavior: smooth;
  overflow: auto;
  /* background: linear-gradient(to top, #008aff, #00ffe7); */
  animation: anime 5s linear infinite;
  border-radius: 5px;
}

@keyframes animate {
  0%,
  100% {
    filter: hue-rotate(0deg);
  }
  50% {
    filter: hue-rotate(360deg);
  }
}

.scroll-bar::before {
  content: "";
  position: absolute;

  background: linear-gradient(to top, #008aff, #00ffe7);
  filter: blue(10px);
}
.scroll-bar::after {
  content: "";
  position: absolute;

  background: linear-gradient(to top, #008aff, #00ffe7);
  filter: blue(30px);
}

.scroll-bar h5 {
  padding: 0px 5px;
  margin-top: 10px;
}

.scroll-bar a {
  color: black;
}

.content-isi-materi {
  border: 1px solid rgb(218, 215, 215);
  padding: 20px;
  margin: 10px;
  height: auto;
  width: 80%;
}
</style>