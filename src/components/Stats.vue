<template>
<div id="stats">
 
    <div class="project">
    <p class="number" v-for="(project, index) of projects">{{ project }}</p>
    <div class="containerDescription">
    <p class="description">Project Completed</p>
    <p class="description">Github Repository</p>
    </div>
    </div>
    <div class="years">
    <p class = "number" v-for="(year, index) in years">{{ year }}</p>
    <div class="containerDescription">
    <p class="description">Years of Experience</p>
    <p class="description">Youtube Subscribers</p>
    </div>
    </div>
    

</div>

</template>

<script setup lang="ts">import { ref } from '@vue/reactivity';

const projects = ref(['50+','45+']);
const years = ref([ '5+', '700+']);

</script>


<style scoped lang="scss">


.project{
    border-top: 3px solid #F0F0F5;
}
.project, .years {
    width:100%;
    height:112px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 3px solid #F0F0F5;
    .numbers{
        padding:0 38px;
        font-weight: 500;
    }
}


.description{
    font-size: 8px;
    color:#BFB8B8;
   }


</style>