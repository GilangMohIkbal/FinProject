<template>
    <div class="main-sidebar">
        <aside id="sidebar-wrapper">
          <div class="sidebar-brand">
            <a href="index.html">SandBox</a>
          </div>
          <div class="sidebar-brand sidebar-brand-sm">
            <a href="index.html">St</a>
          </div>
          <ul class="sidebar-menu">

              <li v-for="(sidebar, i) in sidebar" :key="i" >
                <!-- <a class="nav-link"  href="blank.html"><i class="far fa-square"></i> <span>{{ list }}</span></a> -->
              <NuxtLink class="nav-link mb-3" :to="sidebar.link">
                <i :class="sidebar.icon"></i> <span>{{sidebar.name}}</span>
                
              </NuxtLink>
              </li>
            </ul>

            
        </aside>
      </div>
</template>

<script>
export default {
  data() {
    return {
      sidebar: [
        {
        name: "Home",
        icon: "fas fa-home",
        link: "/"
      },
       
       {
        name: "Sandbox II Front-end Basic",
        icon: "fas fa-chalkboard-teacher",
        link: "/sandbox2"
      },
       {
        name: "Sandbox III Front-end Advance",
        icon: "fas fa-chalkboard-teacher",
        link: "/sandbox3"
      },
      ],
    };
  },
  
};

</script>