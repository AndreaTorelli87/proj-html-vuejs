<script>
export default {
   name: "PageHeader",
   methods: {
   }
}

</script>

<template>
   <div class="container d-flex justify-content-between p-3 align-items-center fixed-top">
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
               <ul class="navbar-nav">
                  <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
                  <li class="nav-item"><a class="nav-link" href="#">About Us</a></li>
                  <li class="nav-item"><a class="nav-link" href="#">Feature</a></li>
                  <li class="nav-item"><a class="nav-link" href="#">Testimonials</a></li>
                  <li class="nav-item"><a class="nav-link" href="#">Contact US</a></li>
               </ul>
               <div class="icons px-4 fw-bolder">
                  <i class="fa-solid fa-magnifying-glass p-3"></i>
                  <i class="fa-solid fa-cart-shopping p-3"></i>
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
}

.my-header{
   position: fixed;
   top: 0;
   left: 0;
}

</style>