<!-- Please remove this file from your project -->
<template>
  <div class="relative flex min-h-screen bg-gray-100 sm:pt-0 justify-center">
    <script
      src="https://kit.fontawesome.com/c42a906203.js"
      crossorigin="anonymous"
    ></script>
    <div class="w-4/5 lg:px-8 flex items-center flex-col gap-8 my-8">
      <TitleNameSection />
      <Objectives />
      <Experience/>
      <Influence />
      <FooterSocialLinks />
    </div>
  </div>
</template>

<script>
import FooterSocialLinks from './profile-screen/FooterSocialLinks';
import TitleNameSection from './profile-screen/TitleNameSection';
import Objectives from './profile-screen/Objectives';
import Experience from './profile-screen/Experience.vue';
import Influence from './profile-screen/Influence.vue'
export default {
  components: {
    FooterSocialLinks,
    TitleNameSection,
    Objectives,
    Experience,
    Influence
  },
  name: "Protfolio",
};
</script>
<style lang="scss">
.details {
  @apply text-lg;
}
.ant-timeline-item-tail {
  border-left: 3px solid #a0a6f2;
}

</style>
