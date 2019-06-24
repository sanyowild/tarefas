<template>
    <div class="task-grid">
        <task v-for="task in tasks" :key="task.name" :task="task"></task>
    </div>
    
</template>

<script>
import task from './task.vue'
export default {
    components:{task},
   props:{
       tasks:{type:Array, required:true}
   }

}
</script>

<style>

</style>
