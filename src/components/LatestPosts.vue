<script>
export default {
   name: "LatestPosts",
   data() {
      return {
         cards: [19,18,17]
      }
   },
   methods: {
   }
}

</script>

<template>
   <div class="container py-5">
      <div class="text-center p-3">
         <h2>Latest Posts</h2>
         <p>If you planning in developing a product landing.</p>
      </div>
      <div class="d-flex py-5">
         <div class="card position-relative p-2 mx-3" v-for="(card, i) in cards" key="i">
            <img :src="`../../public/img/${card}.jpg`">
            <div class="card-body">
               <h5 class="card-title">Life Lack Meaning</h5>
               <p class="card-text">It is a long established fact that a reader will de distracted by the readable.</p>
               <div class="etichetta position-absolute">November 28, 2019</div>
            </div>
         </div>
      </div>
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
.card{
   width: calc(100% / 3);
}
.etichetta{
   background-color: $primo-bg;
   color: $ottavo-text;
   padding: 0.6rem 1rem;
   border-radius: 0.2rem;
   top: 1rem;
   left: 1rem;
}
</style>