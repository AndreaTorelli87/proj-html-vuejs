<script>
export default {
   name: "OurTestimonials",
   data() {
      return {
         testimonials: [
            { img: 26, name: "Julia Aann", title: " - COO Sofbox" },
            { img: 27, name: "Mac Znder", title: " - Manager Sofbox" }
         ]
      }
   }
}
</script>

<template>
   <div class="sfondo my-5 my-scroll" id="Testimonials">
      <div class="immagineSfondo">
         <div class="container">
            <div class="text-center py-5 mb-5">
               <h2>Our Testimonials</h2>
               <p>If you are planning on developing a product landing app or website, <br /> take a look at this
                  beautiful-crafted</p>
            </div>
            <div class="d-flex">
               <div class="carta shadow p-3 text-center w-50 mx-4 position-relative" v-for="testimonial in testimonials">
                  <img :src="`/img/${testimonial.img}.jpeg`" :alt="'Pic of ' + testimonial.name"
                     class="rounded-circle p-5">
                  <div class="pb-4">
                     <h5 class="d-inline">{{ testimonial.name }}</h5>
                     <span>{{ testimonial.title }}</span>
                  </div>
                  <p class="text-start">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis
                     praesentium vero eos et consectetur accus adip adip.</p>
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
   background: linear-gradient(to bottom, $secondo-bg, $primo-bg);
}

.immagineSfondo {
   background-image: url(/img/15.png);
   background-repeat: no-repeat;
}

.carta {
   transition: all 0.2s;
   background-color: $primo-bg;

   &:hover {
      scale: 1.1;
   }
}

.fa-quote-right {
   font-size: 11rem;
   position: absolute;
   top: 30%;
   left: 35%;
   opacity: 0.1;
}

img {
   height: 10rem;
}</style>