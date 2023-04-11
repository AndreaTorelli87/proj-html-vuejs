<script>
export default {
   name: "PageJumbo",
   methods: {
   }
}

</script>

<template>
   <div class="contenitore d-flex justify-content-between p-5">
      <div class="testo">
         <h1>The biggest platform for your growth</h1>
         <p>There are many variations of passages of Lorem Ipsum available, but majority have suffered alteration in some form</p>
         <div class="my-btn">Read More</div>
      </div>
      <img src="/img/27-1.png" alt="Image Jumbo">
   </div>

</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

.contenitore {
   max-width: 95rem;
   margin: 6rem auto 0;
   background-color: $secondo-bg;
}

.testo{
   width: 40%;
}
</style>