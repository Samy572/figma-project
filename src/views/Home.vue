<template>
<Header class="head"/>
<Hello class="hello"/>
<Counter/>
</template>

<script setup lang="ts">
import Header from '../components/Header.vue'
import Hello from '../components/Hello.vue'
import Counter from '../components/Counter.vue'
</script>

<style scoped lang ="scss">

.head, .hello{
    padding: 29px 33px;
}


</style>