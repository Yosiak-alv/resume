<script setup>
import SkillListComponent from '../SkillListComponent.vue';

</script>
<template>
    <!--Begin Skills ----------------------------------------------------------------------------------------------------->
    <section class="pb-6 mt-0 mb-4 border-b-4 border-gray-300 first:mt-0 break-inside-avoid">
        <!-- To keep in the same column -->
        <section class="break-inside-avoid">
            <h2
                class="mb-2 text-lg font-bold tracking-widest text-gray-700 print:font-normal"
            >
                SKILLS
            </h2>
            <SkillListComponent 
                :skills="['HTML', 'CSS', 'Tailwind CSS', 'Bootstrap', 'JavaScript', 'PHP', 'Laravel', 'Vue.js', 'React.js', 'React Native', 'Inertia.js', 'Node.js', 'Java', 'Python', 'SQL', 'Postgresql', 'MySQL', 'MongoDB', 'Linux', 'Web Design']"
            /> 
        </section>
    </section>
</template>