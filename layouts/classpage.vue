<template>
    <div class="container-full">
    <div class="nav-top">
        <!-- Navbar -->
        <PartialsNavbar />
        <!-- Akhir Navbar -->
    </div>

    <div class="body">
        <div class="side-left">
            <!-- sidebar -->
          <PartialsSidebar-left />
            <!-- akhir sidebar -->
        </div>

        <div class="isi-content">
            <!-- content -->
           <Nuxt />

            <!-- content -->
        </div>
    </div>
</div>
</template>
<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@500;600;700;800&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

.container-full {
    display: flex;
    flex-direction: column;
}

.nav-top {
    position: fixed;
    width: 100%;

}

.body {
    display: flex;
    flex-direction: row;
    width: 100%;
    height: 500px;
    
    box-sizing: border-box;
}

.isi-content {
    
    width: 100%;
    height: auto; 
    padding-left: 100px;
    margin-top: 137px;
    
}

</style>