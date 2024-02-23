<script setup>
import EducationCard from '../EducationCard.vue';
</script>
<template>
    <!--Education -------------------------------------------------------------------------------------------------------->
    <section class="pb-0 mt-2 border-gray-300 first:mt-0 break-inside-avoid">
        <!-- To keep in the same column -->
        <section class="break-inside-avoid">
            <h2
                class="mb-2 text-lg font-bold tracking-widest text-gray-700 print:font-normal"
            >
                EDUCATION
            </h2>
            <!-- school --------------------------------------------------------------------------->
            <EducationCard
                title="Don Bosco University, El Salvador"
                date="January 2020 &ndash; Present"
                type="Computer Science Engineering"
                :itemList="[{
                    major: 'Computer Science',
                    gpa: '3.3',
                    skills: 'Programming, Algorithms, Data Structures, Software Development'
                }]"
            />
            <!--school 2--------------------------------------------------------------------------------------------->
            <EducationCard
                title="Hispanoamerican School, El Salvador"
                date="2018 &ndash; 2019"
                type="High School Education"
                :itemList="[{
                    gpa: '3.7',
                    skills: 'Research, Analysis, Critical Thinking, Communication, Problem Solving, Teamwork'
                }]"
            />
            <!--school 3 --------------------------------------------------------------------------------->
            <EducationCard
                title="Coursera"
                date="Dicember 2022 - January 2023"
                type="Certificates"
                :itemList="[
                    {
                        categories: [
                            {
                                subject: 'Django for Everybody',
                                skills: 'Python, Django, Web Development, Database Management, Software Development'
                            },
                            {
                                subject: 'IBM Python for Data Science & AI',
                                skills: 'Python, Data Science, AI, Machine Learning, Data Analysis'
                            },
                            {
                                subject: 'Java for Android',
                                skills: 'Java, Android, Mobile Development, Android Studio, Software Development'
                            },
                            {
                                subject: 'Python for Everybody',
                                skills: 'Python, Data Strutures, Algorithms, OOP, Databases'
                            },

                        ]
                    }
                ]"
            />
            
            <!--school 4 --------------------------------------------------------------------------------->
            <EducationCard
                title="New Millenium, El Salvador"
                date="Dicember 2019"
                type="Certificate"
                :itemList="[{
                    subject: 'Maintenance and Repair of Computers',
                    skills: 'Computer Repair, Hardware, Software, Networking'
                }]"
            />
            
        </section>
    </section>
</template>