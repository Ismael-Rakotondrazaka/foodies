<template>
  <div class="text-gray-500 from-red-100 bg-gradient-to-br">
    <TheHeader />
    <main>
      <TheHeroSection />
      <TheStepSection />
      <TheMenuSection />
      <TheFeedSection />
      <TheBookingSection />
    </main>
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from "@/components/mains/TheHeader.vue";
import TheFooter from "@/components/mains/TheFooter.vue";
import TheBookingSection from "@/components/sections/TheBookingSection.vue";
import TheHeroSection from "@/components/sections/TheHeroSection.vue";
import TheStepSection from "@/components/sections/TheStepSection.vue";
import TheMenuSection from "@/components/sections/TheMenuSection.vue";
import TheFeedSection from "@/components/sections/TheFeedbackSection.vue";

export default {
  name: "TheHomeMain",
  components: {
    TheHeader,
    TheFooter,
    TheBookingSection,
    TheHeroSection,
    TheStepSection,
    TheMenuSection,
    TheFeedSection,
  },
};
</script>

<style>
</style>