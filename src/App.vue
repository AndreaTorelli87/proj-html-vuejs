<script>
import PageHeader from './components/PageHeader.vue';
import PageJumbo from './components/PageJumbo.vue';
import AboutUs from './components/AboutUs.vue';
import OurFeatures from './components/OurFeatures.vue';
import OurTestimonials from './components/OurTestimonials.vue';
import LatestPosts from './components/LatestPosts.vue';
import OurContact from './components/OurContact.vue';
import PageFooter from './components/PageFooter.vue';

export default {
   components: {
      PageHeader,
      PageJumbo,
      AboutUs,
      OurFeatures,
      OurTestimonials,
      LatestPosts,
      OurContact,
      PageFooter,
   },
   data() {
      return {
         footerLinks: [
            {
               title: "Menu",
               links: ["About Us", "Theme", "Features", "Pricing", "Blog"]
            }, {
               title: "About Us",
               links: ["About Sofbox", "Roadmap", "How it Work", "Team", "News"]
            }, {
               title: "Quick Links",
               links: ["About Sofbox", "Roadmap", "How it Work", "Team", "News"]
            }
         ]
      }
   },
   methods: {
   }
}
</script>

<template>
   <PageHeader />
   <main>
      <PageJumbo />
      <AboutUs />
      <OurFeatures />
      <OurTestimonials />
      <LatestPosts />
      <OurContact />
      <hr />
   </main>
   <PageFooter 
      :footerLinks="footerLinks"
   />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use "./styles/variables.scss" as *;
</style>