<template>
  <div class="skills">
    <h2>Skills</h2>
    <div class="stack" >
          <h3 v-for="(stacks, index) of stack">{{ stacks.name }}</h3>
          
    </div>
  
  </div>
</template>

<script setup lang="ts">

import { ref } from 'vue';


const stack = ref( [
   
   {
       id: 1,
       name: 'HTML'
   },
   {
       id: 2,
       name: 'CSS'
   },
   {
       id: 3,
       name: 'PHP'
   },
  
       {
           id: 4,
           name: 'JavaScript'
       },
       {
           id: 5,
           name: 'Python'
       },
   
   
       {
           id: 6,
           name: 'SQL'
       },
       {
           id:7,
           name: 'C/C++'
       },
       {
           id:8,
           name: 'Typescript'
       },
   
   
       {
           id:'9',
           name:'Responsive Design'
       },
   
   
       {
           id: 10,
           name: 'Node Js'
       },
       {
           id: 11,
           name: 'UI/UX Desgin'
       }
   
   ])


</script>

<style scoped lang="scss">
.skills{
    min-height: 100vh;
}
h2 {
  padding: 30px 0;
  color: #5e3aee;
  text-align: center;
  font-size: 35px;
}

.stack{
  cursor: pointer;
  display: flex;
  flex-direction: columns;
  justify-content: space-around;
  flex-wrap: wrap;


}

h3{
  padding: 15px;
  font-size: 24px;
  line-height: 36px;
  font-weight: 400px;
  margin-bottom: 19px;
}
</style>
