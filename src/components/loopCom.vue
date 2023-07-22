<script setup>
// const items=[1,2,3,4,5]
const tasks=[
    'task one is prepare',
    'task two is prepare',
    'task three is prepare',
    'task four is prepare',
    'task five is prepare'
]
</script>

<template>
   <section class="mx-auto container flex items-center text-center flex-col space-y-2">
    <!-- // show only simple for loop -->
        <!-- <div class="p-5 border border-gray-600 w-40" v-for="item in items" :key="item.id">{{ item }}</div> -->
        <!-- <div class="p-5 border border-gray-600 w-40" v-for="n in 10" :key="n.id">{{ n }}</div> -->
        <!-- // show with index or sl no  -->
        <div class="p-5 border border-gray-600 w-40" v-for="(task,index) in tasks" :key="task.id">{{index+1}} = {{ task }}</div>

    </section>
</template>

<style scoped>

</style>