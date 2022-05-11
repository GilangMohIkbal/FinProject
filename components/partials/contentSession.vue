<template>
  <div class="isi-materi">
    <!-- list materi -->
    <div class="list-materi">
      <div class="title"><p>List of Session</p></div>
      <div class="title-list" id="progressbar">
        <div class="scroll-bar">
          <!--  -->
          <div
            class="nav flex-column nav-pills"
            id="v-pills-tab"
            role="tablist"
            aria-orientation="vertical"
          >
            <h5>Front End Programming</h5>
            <a
              v-for="(item, index) in listSession"
              :key="index"
              class="nav-link"
              :href="'#Session' + item.id"
              data-toggle="pill"
              >{{ item.name }}</a
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
          v-for="(session, index) in listSession"
          :key="index"
          class="tab-pane fade"
          :id="'Session' + session.id"
        >
          <h3>{{ session.name }}</h3>
          <br />
          <h6>Description</h6>
          <p>{{ session.description }}</p>
          <div class="row">
            <div
              v-for="(material, index) in session.listMaterial"
              :key="index"
              class="col-6"
            >
              <div class="card">
                <!-- <img src="..." class="card-img-top" alt="..." /> -->
                <div class="card-body">
                  <h5 class="card-title">{{ material.title }}</h5>
                  <p class="card-text">
                    Some quick example text to build on the card title and make
                    up the bulk of the card's content.
                  </p>
                  <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
              </div>
            </div>
          </div>
          <br>
          <button type="button" class="btn btn-primary btn-lg btn-block">
            + Add Material
          </button>
        </div>
      </div>
    </div>
    <!-- akhir isi content -->
  </div>
</template>
<script>
export default {
  data() {
    return {
      listSession: [
        {
          name: "Session 1",
          id: "1",
          description: "Belajar Front End Programming",
          listMaterial: [
            {
              title: "",
              type: "video",
            },
            {
              title: "CSS",
              type: "pdf",
            },
            {
              title: "JavaScript",
              type: "image",
            },
          ],
        },
        {
          name: "Session 2",
          id: "2",
          description: "Belajar Front End Framework",
          listMaterial: [
            {
              title: "HTML",
              type: "video",
            },
            {
              title: "CSS",
              type: "pdf",
            },
            {
              title: "JavaScript",
              type: "image",
            },
              {
              title: "HTML",
              type: "video",
            },
            {
              title: "CSS",
              type: "pdf",
            },
            {
              title: "JavaScript",
              type: "image",
            },
          ],
        },
      ],
    };
  },
};
</script>

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
  background-color: rgb (9, 212, 150);
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

  background: linear-gradient(to top, #09d496, #00ffe7);
  filter: blue(10px);
}
.scroll-bar::after {
  content: "";
  position: absolute;

  background: linear-gradient(to top, #09d496, #00ffe7);
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
