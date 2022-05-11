<template>  
<body>
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
            <!-- akhir content -->
        </div>
        <div class="side-right">
            <!-- sidebar kanan  -->
            <PartialsSidebar-right />
        </div>
    </div>
</div> 
</body>

</template>

<script>
export default {};
</script>
<style scoped>
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
    height: auto;
    justify-content: space-between;
    box-sizing: border-box;
    
    
}

/* .side-left {
    background-color: rgb(26, 51, 161);
    
    
    
} */

.isi-content {
    
    width: 100%;
    height: auto; 
    padding-left: 200px;
    padding-right: 200px;
    margin-top: 137px;
    
    
   
    
}

.side-right {
    position: fixed;
}

</style>