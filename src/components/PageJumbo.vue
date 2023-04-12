<script>
export default {
   name: "PageJumbo",
   data() {
      return {
         list: [
            "SEO",
            "SEM",
            "Website Strategy",
            "Social management"
         ]
      }
   },
   methods: {
   }
}
</script>

<template>
   <div class="contenitore d-flex justify-content-between p-5 position-relative my-scroll" id="Jumbo">
      <div class="w-50">
         <h1>The biggest platform for your growth</h1>
         <p class="py-2">There are many variations of passages of Lorem Ipsum available, but majority have suffered alteration in some form</p>
         <div class="my-btn">Read More</div>
      </div>
      <img src="/img/27-1.png" alt="Image Jumbo" class="h-100 position-absolute">
   </div>
   <div class="container my-scroll" id="AboutUS">
      <!-- modificare con row e col per togliere il calc -->
      <section class="d-flex p-4 mt-5">
         <div class="carta d-flex p-3" v-for="card in 3">
            <div class="w-50">
               <img src="../../public/img/24.png" alt="logo monitor" class="w-100 p-2">
            </div>
            <div class="ps-2">
               <h3>Online Marketing</h3>
               <p>It is a long enstablished fact that a reader will be distracted.</p>
               <ul>
                  <li v-for="item in list">
                     <i class="fa-solid fa-check"></i>
                     {{ item }}
                  </li>
               </ul>
            </div>
         </div>
      </section>
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

.contenitore {
   max-width: 80rem;
   margin: 6rem auto 0;
   background-color: $secondo-bg;
}

.carta {
   width: calc(100% / 3);
}

.fa-check {
   color: $quinto-text;
}

img{
   top: 2rem;
   right: 3rem;
}
</style>