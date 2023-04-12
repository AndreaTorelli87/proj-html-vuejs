<script>
export default {
   name: "OurTestimonials",
   data() {
      return {
         testimonials: [
            {
               img: 26,
               name: "Julia Aann",
               title:" - COO Sofbox"
            },
            {
               img: 27,
               name: "Mac Znder",
               title:" - Manager Sofbox"
            }
         ]
      }
   },
   methods: {
   }
}

</script>

<template>
   <div class="sfondo my-5" id="Testimonials">
      <div class="immagineSfondo">
         <div class="container my-scroll">
            <div class="text-center py-5">
               <h2>Our Testimonials</h2>
               <p>If you are planning on developing a product landing app or website, <br /> take a look at this beautiful-crafted</p>
            </div>
            <div class="d-flex">
               <div class="carta shadow bg-white p-3 text-center w-50 mx-4 position-relative" v-for="testimonial in testimonials">
                  <img :src="`../../public/img/${testimonial.img}.jpeg`" :alt="'Pic of ' + testimonial.name" class="rounded-circle p-5">
                  <div class="pb-4">
                     <h5 class="d-inline">{{ testimonial.name }}</h5>
                     <span>{{ testimonial.title }}</span>
                  </div>
                  <p class="text-start">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.</p>
                  <i class="fa-solid fa-quote-right"></i>
               </div>
            </div>
         </div>
      </div>
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

.sfondo {
   background: linear-gradient(to bottom, $secondo-bg, white);
}

.immagineSfondo {
   background-image: url(../../public/img/15.png);
   background-repeat: no-repeat;
}

.fa-quote-right {
   font-size: 11rem;
   z-index: 0;
   position: absolute;
   top: 30%;
   left: 35%;
   opacity: 0.1;
}

img {
   height: 10rem;
}
</style>