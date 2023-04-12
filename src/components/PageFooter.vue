<script>

export default {
   name: "PageFooter",
   props: {
      footerLinks: Object,
   },
   data() {
      return {
      }
   },   
   methods: {
   }
}

</script>

<template>
   <div class="container py-5 d-flex position-relative">
      <div>
         <img src="../../public/img/35.png" alt="Logo Sofbox">
         <p class="card-text">It is a long established fact that a reader will de distracted by the readable.</p>
         <p class="pt-3">Copyright @ 2018 <a href="#Home">Sofbox</a></p>
      </div>
      <div class="list ps-5" v-for="(menu, i) in footerLinks" key="i">
         <h4 class="pb-2">{{ menu.title }}</h4>
         <ul class="p-0">
            <li v-for="link in menu.links" class="py-1">{{ link }}</li>
         </ul>
      </div>
      <div class="freccia rounded-circle d-flex align-items-center justify-content-center">
         <a href="#Home">
            <i class="fa-solid fa-chevron-up text-white"></i>
         </a>
      </div>  
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
.container > * {
   width: calc(100% / 4);
}
li{
   color: $quarto-text;
   cursor: pointer;
   transition: all 0.2s;

   &:hover{
      color: $ottavo-text;
   }
}
.freccia{
   background-color: #B2B2B2;
   bottom: 1rem;
   right: -4rem;
   height: 3rem;
   width: 3rem;
   position: absolute;

}
</style>