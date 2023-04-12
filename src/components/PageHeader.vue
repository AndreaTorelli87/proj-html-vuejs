<script>
export default {
   name: "PageHeader",
   props: {
      headerNav: Array,
   },
   methods: {
   }
}
</script>

<template>
   <div class="container d-flex justify-content-around p-3 align-items-center fixed-top bg-white">
      <div>
         <img src="../../public/img/logo-2.png" alt="Logo Softbox">
      </div>
      <nav class="navbar navbar-expand-lg bg-body-tertiary">
         <div class="container-fluid">
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown"
               aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
               <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNavDropdown">
               <ul class="navbar-nav" v-for="(link, i) in headerNav" key="i">
                  <li class="nav-item"><a class="py-2 mx-2 text-decoration-none" :href="'#' + link">{{ link }}</a></li>
               </ul>
               <div class="icons px-4 fw-bolder">
                  <i class="fa-solid fa-magnifying-glass p-3"></i>
                  <i class="fa-solid fa-cart-shopping p-3 position-relative">
                     <span class="position-absolute top-5 start-98 translate-middle badge rounded-pill bg-primary">
                        0
                     </span>
                  </i>
               </div>
               <div class="my-btn">Get Started</div>
            </div>
         </div>
      </nav>
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;


img {
   height: 3rem;
}

a {
   color: $ottavo-text;
   border-bottom: solid 2px white;
   transition: all 0.2s;

   &:hover {
      color: $quinto-text;
      border-bottom: solid 2px $terzo-border;
   }
}

.my-header {
   position: fixed;
   top: 0;
   left: 0;
}
</style>