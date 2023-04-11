<script>
export default {
   name: "PageJumbo",
   methods: {
   }
}

</script>

<template>
   <div class="contenitore d-flex justify-content-between p-5 position-relative">
      <div class="w-50">
         <h1>The biggest platform for your growth</h1>
         <p class="py-2">There are many variations of passages of Lorem Ipsum available, but majority have suffered alteration in some form</p>
         <div class="my-btn">Read More</div>
      </div>
      <img src="/img/27-1.png" alt="Image Jumbo" class="h-100 position-absolute">
   </div>

</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

.contenitore {
   max-width: 80rem;
   margin: 6rem auto 0;
   background-color: $secondo-bg;
}

img{
   top: 2rem;
   right: 3rem;
}
</style>