<script setup>
import ExperienceCard from '../ExperienceCard.vue'
</script>
<template>
    <section class="pb-2 pb-4 mt-4 border-b-4 border-gray-300 first:mt-0">
        <!-- To keep in the same column ------------------------------------------------------------------------->
        <section class="break-inside-avoid">
            <h2 class="mb-2 text-xl font-black tracking-widest text-gray-800 print:font-normal">
                EXPERIENCE
            </h2>
            <!--Job 1--> 
           <ExperienceCard
                title="Full Stack Web Developer"
                :date="{start: 'Nov 2023', end: 'Feb 2024'}"
                company="Fe y Alegría, El Salvador"
                :descriptions="[
                    'Created high-quality, customized web applications from scratch, employing a diverse set of programming languages, including HTML, CSS, JavaScript and PHP, to fulfill unique client requirements.',
                    'Leveraged a range of bleeding edge front-end frameworks like Vue.js, as well as back-end framework such as Laravel, to deliver robust and scalable web solutions.',
                    'Designed and implemented databases using SQL and NoSQL technologies like MySQL, PostgreSQL and MongoDB, optimizing data storage and management.'
                ]"
            />
            <!-- job 2  -->
            <ExperienceCard
                title="Technical Support Assistant"
                :date="{start: 'Aug 2022', end: 'Feb 2023'}"
                company="Fe y Alegría, El Salvador"
                :descriptions="[
                    'Provided expert computer repair services, effectively diagnosing and resolving hardware and software issues.',
                    'Demonstrated proficiency across diverse operating systems (Windows, Linux) and hardware components, offering tailored solutions, including hardware upgrades, software installations, and malware removal.',
                ]"
                :without-border="true"
            />
        </section>
    </section>

</template>