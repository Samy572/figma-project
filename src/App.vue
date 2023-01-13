<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import Home from '../src/views/Home.vue'
import About from '../src/views/About.vue'
import Skills from './views/Skills.vue';
import Contact from './views/Contact.vue';
</script>

<template>
 <Home/>
 <About/>
  <Skills/>
  <Contact/>
</template>

<style scoped lang="scss">

</style>
