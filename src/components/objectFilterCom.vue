<script setup>
    const tasks=[
    {id:1,title:"Task one done",status:"done"}, 
    {id:2,title:"Task two pending",status:"pending"},   
    {id:3,title:"Task three done",status:"done"},   
    {id:4,title:"Task four processing",status:"processing"}, 
    {id:5,title:"Task five processing",status:"processing"}  
    ]

    function taskDone(){
        return tasks.filter(task=>"done"==task.status)
    }
</script>

<template>
   <section class="mx-auto container flex items-center text-center flex-col space-y-2">
 
        <!-- <div class="p-5 border border-gray-600 w-40" v-for="task in tasks" :key="task.id">{{task.id}} = {{ task.title }}</div> -->
        <div class="p-5 border border-gray-600 w-40" v-for="task in taskDone()" :key="task.id">{{task.id}} = {{ task.title }}</div>

    </section>
</template>

<style scoped>

</style>