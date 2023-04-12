<script>
export default {
   name: "OurTestimonials",
   methods: {
   }
}

</script>

<template>
   <div class="sfondo my-5" id="Testimonials">
      <div class="container my-scroll">
         <div class="text-center py-5">
            <h2>Our Testimonials</h2>
            <p>If you are planning on developing a product landing app or website, <br /> take a look at this beautiful-crafted</p>
         </div>
         <div class="d-flex">
            <!-- dinamicizza creazione carte e aggiungi virgolette giganti di sfondo-->
            <div class="carta shadow bg-white p-3 text-center w-50 mx-4">
               <img src="../../public/img/26.jpeg" alt="Pic of Julia Aann" class="rounded-circle p-5">
               <div class="pb-4">
                  <h5 class="d-inline">Julia Aann</h5>
                  <span> - COO Sofbox</span>
               </div>
               <p class="text-start">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.</p>
            </div>
            <div class="carta shadow bg-white p-3 text-center w-50 mx-4">
               <img src="../../public/img/26.jpeg" alt="Pic of Julia Aann" class="rounded-circle p-5">
               <div class="pb-4">
                  <h5 class="d-inline">Julia Aann</h5>
                  <span> - COO Sofbox</span>
               </div>
               <p class="text-start">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.</p>
            </div>
         </div>
      </div>
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

.sfondo{
   background-image: url(../../public/img/15.png);
   background-repeat: no-repeat;
   background-color: $secondo-bg;
}

img{
   height: 10rem;
}

</style>