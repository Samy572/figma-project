<template>
    <div class="counter">
     <div class="container--counter" v-for="(counters, index) of counter" :key="index">
        <div class="wrapper">
            <h2>{{ counters[0].title }}+</h2>
             <p>{{ counters[0].content }}</p>
        </div>
        <div class="separator"></div>
        <div class="wrapper">
             <h2>{{ counters[1].title }}+</h2>
             <p>{{ counters[1].content }}</p>
        </div>
    </div>
  </div>
</template>

<script setup lang="ts">import { ref } from '@vue/reactivity';

const counter = ref([[
    {
        title: '50',
        content: 'Projects Completed',
    },
    {
        title: '45',
        content: 'Github Repository'
    }
],
[
    {
        title: '5',
        content: 'Year Experiences'
    },
    {
        title: '700',
        content: 'Youtube Subscribers'
    }
]])


</script>


<style scoped lang="scss">
.counter{
    display: flex;
    justify-content: center;
    width:100%;
    text-align: center;
}
.container--counter{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    border-bottom: 3px solid #BFB8B8;
    border-top: 3px solid #BFB8B8;
    padding: 10px 0;
    height:224px;
    p{
        font-size: 8px;
        color: #BFB8B8;
    }
}

.separator{
    width: 100%;
    background-color: #BFB8B8;
    height: 3px;
}

</style>