<template>
  <div class="isi-materi">
    <!-- list materi -->
    <div class="list-materi">
      <div class="title"><p>List Materi</p></div>
      <div class="title-list" id="progressbar">
        <div class="scroll-bar">
          <!--  -->
          <div
            class="nav flex-column nav-pills"
            id="v-pills-tab"
            role="tablist"
            aria-orientation="vertical"
          >
          <h5>String & Integer</h5>
          
            <a
              class="nav-link"
              id="v-pills-pengantar-tab"
              data-toggle="pill"
              href="#v-pills-pengantar"
              role="tab"
              aria-controls="v-pills-pengantar"
              aria-selected="true"
              >Pengantar</a
            >
            <a
              class="nav-link"
              id="v-pills-console-tab"
              data-toggle="pill"
              href="#v-pills-console"
              role="tab"
              aria-controls="v-pills-console"
              aria-selected="false"
              >Console.log</a
            >
            <a
              class="nav-link"
              id="v-pills-kalkulasi-tab"
              data-toggle="pill"
              href="#v-pills-kalkulasi"
              role="tab"
              aria-controls="v-pills-kalkulasi"
              aria-selected="false"
              >Kalkulasi</a
            >
            <a
              class="nav-link"
              id="v-pills-string-tab"
              data-toggle="pill"
              href="#v-pills-string"
              role="tab"
              aria-controls="v-pills-string"
              aria-selected="false"
              >String</a>

             <h5>Variabel JavaScript</h5>
          
            <a
              class="nav-link"
              id="v-pills-variabel-tab"
              data-toggle="pill"
              href="#v-pills-variabel"
              role="tab"
              aria-controls="v-pills-variabel"
              aria-selected="false"
              >Variabel</a
            >
            <a
              class="nav-link"
              id="v-pills-tipe-tab"
              data-toggle="pill"
              href="#v-pills-tipe"
              role="tab"
              aria-controls="v-pills-tipe"
              aria-selected="false"
              >Tipe Data</a
            >
            <a
              class="nav-link"
              id="v-pills-numerik-tab"
              data-toggle="pill"
              href="#v-pills-numerik"
              role="tab"
              aria-controls="v-pills-numerikk"
              aria-selected="false"
              >Tipe Numerik</a
            >
            <a
              class="nav-link"
              id="v-pills-boolean-tab"
              data-toggle="pill"
              href="#v-pills-boolean"
              role="tab"
              aria-controls="v-pills-boolean"
              aria-selected="false"
              >Boolean</a
            >

            <a
              class="nav-link"
              id="v-pills-operator-tab"
              data-toggle="pill"
              href="#v-pills-operator"
              role="tab"
              aria-controls="v-pills-operator"
              aria-selected="false"
              >operato Aritmatik</a
            >
            <h5>Variabel JavaScript</h5>
          
            <a
              class="nav-link"
              id="v-pills-variabel-tab"
              data-toggle="pill"
              href="#v-pills-variabel"
              role="tab"
              aria-controls="v-pills-variabel"
              aria-selected="false"
              >Variabel</a
            >
            <a
              class="nav-link"
              id="v-pills-tipe-tab"
              data-toggle="pill"
              href="#v-pills-tipe"
              role="tab"
              aria-controls="v-pills-tipe"
              aria-selected="false"
              >Tipe Data</a
            >
            <a
              class="nav-link"
              id="v-pills-numerik-tab"
              data-toggle="pill"
              href="#v-pills-numerik"
              role="tab"
              aria-controls="v-pills-numerikk"
              aria-selected="false"
              >Tipe Numerik</a
            >
            <a
              class="nav-link"
              id="v-pills-boolean-tab"
              data-toggle="pill"
              href="#v-pills-boolean"
              role="tab"
              aria-controls="v-pills-boolean"
              aria-selected="false"
              >Boolean</a
            >

            <a
              class="nav-link"
              id="v-pills-operator-tab"
              data-toggle="pill"
              href="#v-pills-operator"
              role="tab"
              aria-controls="v-pills-operator"
              aria-selected="false"
              >operato Aritmatik</a
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
          <h3>Pengantar</h3>
          <p>
            Javascript diperkenalkan pertama kali oleh Netscape pada tahun 1995.
            Pada awalnya bahasa ini dinamakan “LiveScript” yang berfungsi
            sebagai bahasa sederhana untuk browser Netscape Navigator 2. Pada
            masa itu bahasa ini banyak di kritik karena kurang aman,
            pengembangannya yang terkesan buru buru dan tidak ada pesan
            kesalahan yang di tampilkan setiap kali kita membuat kesalahan pada
            saat menyusun suatu program. Kemudian sejalan dengan sedang giatnya
            kerjasama antara Netscape dan Sun (pengembang bahasa pemrograman
            “Java” ) pada masa itu, maka Netscape memberikan nama “JavaScript”
            kepada bahasa tersebut pada tanggal 4 desember 1995. Pada saat yang
            bersamaan Microsoft sendiri mencoba untuk mengadaptasikan teknologi
            ini yang mereka sebut sebagai “Jscript” di browser Internet Explorer
            3. Javascript adalah bahasa yang berbentuk kumpulan skrip yang pada
            fungsinya berjalan pada suatu dokumen HTML, sepanjang sejarah
            internet bahasa ini adalah bahasa skrip pertama untuk web. Bahasa
            ini adalah bahasa pemrograman untuk memberikan kemampuan tambahan
            terhadap bahasa HTML dengan mengijinkan pengeksekusian perintah
            perintah di sisi user, yang artinya di sisi browser bukan di sisi
            server web. Javascript bergantung kepada browser(navigator) yang
            memanggil halaman web yang berisi skrip skrip dari Javascript dan
            tentu saja terselip di dalam dokumen HTML. Javascript juga tidak
            memerlukan kompilator atau penterjemah khusus untuk menjalankannya
            (pada kenyataannya kompilator Javascript sendiri sudah termasuk di
            dalam browser tersebut). Lain halnya dengan bahasa “Java” (dengan
            mana JavaScript selalu di banding bandingkan) yang memerlukan
            kompilator khusus untuk menterjemahkannya di sisi user/klien.
          </p>
        </div>
        <div
          class="tab-pane fade"
          id="v-pills-console"
          role="tabpanel"
          aria-labelledby="v-pills-profile-tab"
        >
          <h3>Mengenal Console JavaScript</h3>
          <p>
            anyak orang yang mengatakan, “Belajar JavaScript itu susah, tidak
            seperti belajar HTML. Sebab saat melihat hasilnya di web browser,
            pesan error-nya tidak tampil.” Pendapat ini tidak benar ya karena
            kamu bisa melihatnya melalui console. Buka terlebih dahulu Google
            Chrome, kemudian klik kanan pilih “Inspect” -> Console.
          </p>
        </div>
        <div
          class="tab-pane fade"
          id="v-pills-kalkulasi"
          role="tabpanel"
          aria-labelledby="v-pills-messages-tab"
        >
          ini halaman messages
        </div>
        <div
          class="tab-pane fade"
          id="v-pills-string"
          role="tabpanel"
          aria-labelledby="v-pills-settings-tab"
        >
          ini halaman settings
        </div>

        <div
          class="tab-pane fade"
          id="v-pills-variabel"
          role="tabpanel"
          aria-labelledby="v-pills-variabel-tab"
        >
          Variabel adalah empat dimana kita menyimpan nilai-nilai atau
          informasi-informasi pada JavaScript. Variabel yang dideklarasikan
          dapat di isi dengan nilai apa saja. Dalam JavaScript pendeklarasian
          sebuah variabel sifatnya opsional, artinya anda boleh mendeklarasikan
          atau tidak hal tersebut tidak menjadi masalah. Jika anda memberi nilai
          pada variabel, maka dalam JavaScript dianggap bahwa anda telah
          mendeklarasikan variabel tersebut.
        </div>

        <div
          class="tab-pane fade"
          id="v-pills-tipe"
          role="tabpanel"
          aria-labelledby="v-pills-tipe-tab"
        >
          Tidak seperti bahasa pemrograman lainnya, JavaScript tidak memiliki
          tipe data secara explisit. Hal ini dapat dilihat dari beberapa contoh
          variabel diatas. Anda mendeklarasikan variabel tapi tidak menentukan
          tipenya. Meskipun JavaScript tidak memiliki tipe data secara explisit.
          JavaScript mempunyai tipe data implisit
        </div>

        
        <div
          class="tab-pane fade"
          id="v-pills-numerik"
          role="tabpanel"
          aria-labelledby="v-pills-numerik-tab"
        >
          Pada dasarnya JavaScript hanya mengenal dua macam tipe numerik, yaitu
          bilangan bulat (integer) dan bilangan pecahan(real/float). Untuk
          bilangan bulat, kita dapat merepresentasikan dengan basis desimal,
          oktal atau heksadesimal.
        </div>

        <div
          class="tab-pane fade"
          id="v-pills-boolean"
          role="tabpanel"
          aria-labelledby="v-pills-boolean-tab"
        >
          Tipe boolean hanya mempunyai nilai True atau False. Tipe ini biasanya
          digunakan untuk mengecek suatu kondisi atau keadaan
        </div>

        <div
          class="tab-pane fade"
          id="v-pills-operator"
          role="tabpanel"
          aria-labelledby="v-pills-operator-tab"
        >
          Digunakan untuk operan beripe numerik. Ada dua macam operator
          aritmatik, yaitu operator numerik tunggal dan operator aritmatik
          biner. Perbedaan kedua operator terletak pada jumlah operan yang harus
          dioperasikan.
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