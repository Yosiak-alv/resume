<script setup>

const props = defineProps({
    title: String,
    date: Object,
    company: String,
    descriptions: Array,
    withoutBorder: {
        type: Boolean,
        default: false
    }
})
</script>

<template>
     <section class="mb-2  break-inside-avoid" :class="{'border-b-2 border-gray-300': !withoutBorder}">
        <header>
            <h3 class="font-semibold text-gray-800 text-md leading-snugish">
                {{props.title}}
            </h3>
            <p class="text-sm leading-normal text-gray-500">
                {{props.date.start}} &ndash; {{props.date.end}} | {{props.company}}
            </p>
        </header>
        <ul class="pl-3 mt-2 font-normal text-gray-700 text-md leading-snugish">
            <li v-for="description in props.descriptions">
                <span class="text-gray-500 transform -translate-y-px select-none">
                    &rsaquo;
                </span>
                {{description}}
            </li>
        </ul>
    </section>
</template>