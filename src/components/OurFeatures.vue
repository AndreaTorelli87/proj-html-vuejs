<script>
export default {
   name: "OurFeatures",
   data() {
      return {
         cards: [
            { title: "Customized Invoices", icon: "file-invoice-dollar" },
            { title: "Stock Management", icon: "arrow-trend-up" },
            { title: "Receivable & Payables", icon: "arrows-turn-to-dots" },
            { title: "Manage Buyng", icon: "money-bill-wave" },
            { title: "Powerful & Secure", icon: "lock" },
            { title: "Fastest Return Filing", icon: "gauge-high" },
            { title: "Monthly Detailed", icon: "file-pen" },
            { title: "Product Management", icon: "thumbs-up" }
         ]
      }
   },
   methods: {
      generaColoreRandom() {
         let characters = "0123456789abcdef"
         let str = "#"
         for (let i = 0; i < 6; i++) {
            str += characters[Math.floor(Math.random() * 16)]
         }
         return str;
      }
   }
}
</script>

<template>
   <div class="sfondo my-scroll pb-5" id="Feature">
      <div class="container">
         <div class="d-flex justify-content-between">
            <div class="mt-3">
               <h2>Popular features that your business needs</h2>
               <p>Faff about only a quid blower I don't want no agro bleeding chimney <br /> pot burke tosser cras nice one
                  boot fanny.!</p>
            </div>
            <a class="my-btn m-5 text-decoration-none">Explore More Feature</a>
         </div>
         <div class="d-flex flex-wrap">
            <div class="carta shadow m-2 p-3" v-for="card in cards">
               <h5>{{ card.title }}</h5>
               <div>
                  <i :class="`fa-solid fa-${card.icon}`" :style="`color: ${generaColoreRandom()};`"></i>
               </div>
            </div>
         </div>
      </div>
   </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

.sfondo {
   background-image: url(/img/14.png);
   background-repeat: no-repeat;
   background-size: contain;
   background-position-x: -14rem;
}

.carta {
   width: calc(100% / 4 - 1rem);
   transition: all 0.2s;

   i {
      font-size: 3rem;
      padding: 0.5rem 0;
   }

   ;

   &:hover {
      background-color: #8AE1CE;
      color: $primo-text;
      scale: 1.1;

      i {
         color: $primo-text !important;
      }
   }
}</style>