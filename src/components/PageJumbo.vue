<script>
export default {
   name: "PageJumbo",
   data() {
      return {
         list: ["SEO", "SEM", "Website Strategy", "Social management"]
      }
   }
}
</script>

<template>
   <div class="contenitore d-flex justify-content-between p-5 position-relative my-scroll" id="Home">
      <div class="w-50 pb-5">
         <h1>The biggest platform for your growth</h1>
         <p class="py-2">There are many variations of passages of Lorem Ipsum available, but majority have suffered
            alteration in some form</p>
         <div class="my-btn mt-4">Read More</div>
      </div>
      <img src="/img/27-1.png" alt="Image Jumbo" class="position-absolute">
   </div>
   <div class="container my-scroll d-flex p-5 my-3" id="About us">
      <div class="carta d-flex pe-5" v-for="card in 3">
         <div class="w-25 text-end">
            <img src="/img/24.png" alt="logo monitor" class="w-100">
         </div>
         <div class="ps-2">
            <h3>Online Marketing</h3>
            <p>It is a long enstablished fact that a reader will be distracted.</p>
            <ul class="p-0">
               <li v-for="item in list">
                  <i class="fa-solid fa-check pe-2"></i>
                  {{ item }}
               </li>
            </ul>
         </div>
      </div>
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

.contenitore {
   max-width: 90rem;
   margin: 7rem auto;
   background-color: $secondo-bg;

   img {
      top: 2rem;
      right: 3rem;
   }
}

h1 {
   font-size: 4rem;
}

.carta {
   width: calc(100% / 3);
}

.fa-check {
   color: $quinto-text;
}</style>