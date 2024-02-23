<script setup>
import HeaderComponent from './components/HeaderComponent.vue';
import ContactComponent from './components/ContactComponent.vue';
import SummarySection from './components/sections/SummarySection.vue';
import EducationSection from './components/sections/EducationSection.vue';
import SkillsSection from './components/sections/SkillsSection.vue';
import ExperienceSection from './components/sections/ExperienceSection.vue';
</script>

<template>
  <main class="font-jost hyphens-manual">
    <section
      class="p-3 my-auto mx-auto max-w-3xl bg-gray-100 rounded-2xl border-4 border-gray-700 sm:p-9 md:p-16 lg:mt-6 print:border-0 page print:max-w-letter print:max-h-letter print:mx-0 print:my-o xsm:p-8 print:bg-white md:max-w-letter md:h-letter lg:h-letter"
    >
      <HeaderComponent/>
      <!-- Column -------------------------------------------------------------------------------------------------->
      <section
        class="col-gap-8 print:col-count-2 print:h-letter-col-full col-fill-balance md:col-count-2 md:h-letter-col-full"
      >
        <ContactComponent/>
        <SummarySection/>
        <EducationSection/>
        <SkillsSection/>
        <ExperienceSection/>
      </section>
      
    </section>
  </main>
</template>


