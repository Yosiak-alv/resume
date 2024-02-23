<script setup>
    const props = defineProps({
        skills: Array,
    })
</script>
<template>
    <section class="mb-0 break-inside-avoid">
        <section class="mt-1 last:pb-1">
            <ul class="flex flex-wrap -mb-1 font-bold leading-relaxed text-md -mr-1.6">
                <li class="p-1.5 mb-1 leading-relaxed text-white bg-gray-800 mr-1.6 print:bg-white print:border-inset" v-for="skill in skills">
                    {{skill}}
                </li>
            </ul>
        </section>
    </section>
</template>