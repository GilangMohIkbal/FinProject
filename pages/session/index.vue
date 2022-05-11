<template>
    <div class="content-materi">
                <div class="header-materi">
                    <div class="judul-materi">
                        <div class="icon-materi"></div>
                        <div class="text-icon"><h3>Front End</h3>
                        <p>Start Date : 1 April 2020</p>
                        <p>End Date : 1 April 2020</p>
                        </div>
                    </div>
                </div>
                <!-- isi content -->
                   <PartialsContentSession />
                
                <!-- isi content -->
                 <div
                class="modal fade"
                id="tambahStudent"
                tabindex="1"
                aria-labelledby="exampleModalLabel"
                aria-hidden="true"
              >
                <div class="modal-dialog">
                  <div class="modal-content">
                    <AddStudent />
                  </div>
                </div>
              </div>

               <div
                class="modal fade"
                id="tambahTeacher"
                tabindex="1"
                aria-labelledby="exampleModalLabel"
                aria-hidden="true"
              >
                <div class="modal-dialog">
                  <div class="modal-content">
                    <AddTeacher />
                  </div>
                </div>
            </div>
          </div>
</template>

<script>
export default {
    layout:'sessionpage'
}
</script>

<style scoped>
.content-materi {
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.header-materi {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    border-bottom: 0.5px solid rgb(192, 190, 190);
    padding-bottom: 30px;
}

.judul-materi {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}

.judul-materi .text-icon h3 {
    padding: 10px;
    font-size: 30px;
}
.judul-materi .text-icon p {
    padding: 0px 15px;
    font-size: 15px;
    color: rgb(107, 107, 107);
}

.judul-materi .icon-materi {
    width: 100px;
    height: 100px;
    background-image: url(../../assets/img/javascript.jpg);
    background-size: cover;
    background-position: center;
    
    border-radius: 20px;
}

.isi-materi {
    display: flex;
    flex-direction: row;
    margin-top: 20px;
    
    
    
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

.list-materi .title-list  ul {
    padding-left: 0rem;
    
}
.list-materi .title-list  ul li {

 list-style: none;
 margin: 10px 0;
 text-align: center;
 padding: 0px 5px;
 
}

.list-materi .title-list  ul li a {
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

.list-materi .title-list  ul li a:hover {
    background-color: rgb(190, 216, 236);
    margin-top: 5px;
    margin-bottom: -5px;
    box-shadow: 12px 11px 5px -10px rgba(0,0,0,0.19);
-webkit-box-shadow: 12px 11px 5px -10px rgba(0,0,0,0.19);
-moz-box-shadow: 12px 11px 5px -10px rgba(0,0,0,0.19);
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
    0%,100% {
        filter: hue-rotate(0deg);
    }
    50% {
        filter:hue-rotate(360deg);
    }
  }

  .scroll-bar::before {
    content: '';
    position: absolute;
    
    
    background: linear-gradient(to top, #008aff, #00ffe7);
    filter: blue(10px);
  }
  .scroll-bar::after {
    content: '';
    position: absolute;
    
    
    background: linear-gradient(to top, #008aff, #00ffe7);
    filter: blue(30px);
  }

  .scroll-bar h5 {
      padding: 0px 5px;
  }

  .content-isi-materi {
      border: 1px solid rgb(218, 215, 215);
      padding: 20px;
      margin: 10px;
      height: auto;
      width: 80%;
      
  }

</style>
