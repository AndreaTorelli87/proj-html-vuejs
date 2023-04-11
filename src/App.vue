<script>
import PageHeader from './components/PageHeader.vue';
import PageJumbo from './components/PageJumbo.vue';
import AboutUs from './components/AboutUs.vue';
import OurFeatures from './components/OurFeatures.vue';
import OurTestimonials from './components/OurTestimonials.vue';
import OurContact from './components/OurContact.vue';
import PageFooter from './components/PageFooter.vue';

export default {
   components: {
      PageHeader,
      PageJumbo,
      AboutUs,
      OurFeatures,
      OurTestimonials,
      OurContact,
      PageFooter,
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
      <PageHeader />
      <PageJumbo />
   <div class="container">
      <AboutUs />
      <OurFeatures />
      <OurTestimonials />
      <OurContact />
      <PageFooter />
   </div>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use "./styles/variables.scss" as *;


</style>
