<script>
export default {
   name: "OurContact",
   data() {
      return {
         icons: ["fa-facebook-f", "fa-twitter", "fa-github", "fa-instagram"]
      }
   }
}

</script>

<template>
   <div class="container my-scroll mb-5" id="Contact US">
      <div class="text-center py-5">
         <h2>Contact with our team</h2>
         <p>If you planning in developing a product landing.</p>
      </div>
      <div class="d-flex py-4">
         <div class="pe-5">
            <img src="/img/StaticMapService.GetMapIma.png" alt="Mappa">
         </div>
         <div>
            <img src="/img/35.png" alt="Logo Sofbox" class="pb-5">
            <h5 class="pb-3">9840 Shore st. Fond Du Lac, WI 54935</h5>
            <span>0 1223 456 789</span>
            <br />
            <span>mail@sofbox.com</span>
            <div class="py-5">
               <i v-for="icon in icons" :class="`fa-brands ${icon} cp`"></i>
            </div>
            <h4 class="pb-2">Get in Touch</h4>
            <div>
               <div class="mb-4 d-flex">
                  <div>
                     <input type="text" class="form-control" placeholder="Your Name">
                  </div>
                  <div class="ms-4">
                     <input type="email" class="form-control" placeholder="Your Email">
                  </div>
               </div>
               <div class="mb-4">
                  <input type="text" class="form-control" placeholder="Your Subject">
               </div>
               <textarea class="form-control" placeholder="Your Message" rows="7"></textarea>
               <div class="my-btn mt-4">Send Message</div>
            </div>
         </div>
      </div>
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

.fa-brands {
   margin-right: 0.5rem;
   padding: 0.7rem;
   border-radius: 3px;
   border: solid 1px lightgray;
   width: 40px;
   text-align: center;
   color: $quinto-text;
   transition: all 0.2s;

   &:hover {
      scale: 1.2;
   }
}
</style>