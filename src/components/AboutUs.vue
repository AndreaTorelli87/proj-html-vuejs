<script>
export default {
   name: "AboutUs",

   methods: {
   }
}
</script>

<template>
   <div class="container d-flex">
      <div class="testo w-50">
         <div>
            <h2>Get tips tricks on how to skyrocket your sales.</h2>
            <p>Faff about only a quid blower I don't want no agro bleeding chimney pot burke tosser cras nice one boot
               fanny.!</p>
         </div>
         <div class="tip d-flex align-items-center p-3 mb-4">
            <img src="../../public/img/510.png" class="p-2">
            <div>
               <h4>Reporting Analysis</h4>
               <p>It is a long established fact that a reader will be distracted by the readable content of a page when
                  looking at its layout.</p>
            </div>
         </div>
         <div class="tip d-flex align-items-center p-2">
            <img src="../../public/img/511.png" class="p-2">
            <div>
               <h4>Technical SEO Audit</h4>
               <p>It is a long established fact that a reader will be distracted by the readable content of a page when
                  looking at its layout.</p>
            </div>
         </div>
      </div>
      <div class="ps-3">
         <img src="../../public/img/509.jpeg">
      </div>
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

section {
   margin: 8rem 0;
}
.tip {
   transition: all 0.2s;

   &:hover {
      box-shadow: 0.5rem 1.5rem 1rem rgba(0, 0, 0, 0.15);
      scale: 1;

      h4 {
         color: $quinto-text;
      }
   }
}
</style>