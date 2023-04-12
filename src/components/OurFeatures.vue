<script>
export default {
   name: "OurFeatures",
   data() {
      return {
         cards: [
            "Customized Invoices",
            "Stock Management",
            "Receivable & Payables",
            "Manage Buyng",
            "Powerful & Secure",
            "Fastest Return Filing",
            "Monthly Detailed",
            "Product Management"
         ]
      }
   },
   methods: {
   }
}
</script>

<template>
   <div class="sfondo my-scroll" id="Feature">
      <div class="container">
         <div class="d-flex justify-content-between">
            <div class="mt-3">
               <h2>Popular features that your business needs</h2>
               <p>Faff about only a quid blower I don't want no agro bleeding chimney <br/> pot burke tosser cras nice one boot fanny.!</p>
            </div>
            <div class="my-btn m-5">Explore More Feature</div>
         </div>
         <div class="d-flex flex-wrap">
            <div class="carta shadow m-2 p-3" v-for="(card, i) in cards" key="i">
               <h5>{{ cards[i] }}</h5>
               <div class="">
                  <img src="../../public/img/loader.gif" class="">
               </div>
            </div>
         </div>
      </div>
   </div>   
</template>

<style lang="scss" scoped>
   .sfondo{
      background-image: url(../../public/img/14.png);
      background-repeat: no-repeat;
      background-size: contain;
      background-position: left;
   }

   .carta{
      width: calc(100% / 4 - 1rem);
      img {
         height: 5rem
      };
   }

</style>