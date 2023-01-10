<template>
  <header>
    <img src="../assets/images/logo.svg" alt="reboot13" />
    <div class="burger"  @click="state = !state" :class="{'open' : state}">
      <div class="ligne" ></div>
      <div class="ligne"></div>
      <div class="ligne"></div>
    </div>

    <div class="menu" :class= "{'menuShow': state}"></div>
  </header>
</template>

<script setup lang="ts">
import { ref } from "@vue/reactivity";

const state = ref(false);

</script>

<style scoped lang="scss">
@import "../assets/sass/base.scss";

header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  .burger{
    cursor: pointer;
    .ligne {
     width: 23px;
     height: 3px;
     background-color: rgb(23, 23, 23);
     margin-top: 3px;
     
    }
  }
  
}





.menu {
  position: fixed;
  top: 0%;
  left: 100%;
  min-height: 100vh;
  background-color: rgb(32, 31, 31);
  width: 100vw;
  transition: 0.3s;
}

.menuShow {
    left:0%;
}

.open{
    background-color: white;
    z-index: 2;
}
</style>
