<script setup>
    const props = defineProps({
        title: String,
        date: String,
        type: String,
        itemList: Array,
       
    });
</script>

<template>
     <div class="pb-2 mb-2 border-b-2 break-inside-avoid">
        <header>
            <h3
                class="flex-grow text-lg font-semibold text-gray-700 leading-snugish"
            >
                {{props.title}}
            </h3>
            <p class="leading-normal text-gray-500 text-md">
                {{props.date}} | {{props.type}}
            </p>
        </header>
        <ul class="mt-2 list-disc list-inside text-gray-800 text-md" v-for="item in props.itemList">
            <div v-if="item.categories != null " v-for="category in item.categories" :key="category.subject">
                <span
                    class="font-semibold text-md"
                >
                Subject:
                </span>
                {{category.subject}}
                <li>
                    <span
                        class="font-semibold text-md"
                    >
                        Skills:
                    </span>
                   {{category.skills}}
                </li>
            </div>
            <li v-if="item.major" >
                <span
                    class="font-semibold text-md"
                >
                Major:
                </span>
                {{item.major}}
            </li>
            <li v-if="item.gpa">
                <span
                    class="font-semibold text-md"
                >
                    GPA:
                </span>
                {{item.gpa}}
            </li>
            <li v-if="item.subject">
                <span
                    class="font-semibold text-md"
                >
                    Subject:
                </span>
                {{item.subject}}
            </li>
            <li v-if="item.skills">
                <span
                    class="font-semibold text-md"
                >
                    Skills:
                </span>
                {{item.skills}}
            </li>
        </ul>
    </div>
</template>