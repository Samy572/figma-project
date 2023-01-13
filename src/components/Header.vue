<template>
  <header>
    <img src="../assets/images/logo.svg" alt="reboot13" />
    <div class="burger"  @click="state = !state" :class="{'open' : state}">
      <div class="ligne" ></div>
      <div class="ligne"></div>
      <div class="ligne"></div>
    </div>

    <div class="menu" :class= "{'menuShow': state}">
    <nav>
        <ul>
            <li v-for="(menus, index) of menu" :key="index">{{ menus.list }}</li>
        </ul>
    </nav>
    </div>
  </header>
</template>

<script setup lang="ts">
import { ref } from "@vue/reactivity";
const menu = ref([
  {
    list: 'Home'
  },
  {
    list: 'Project'
  },
  {
    list: 'About'
  },
  {
    list: 'Contact'
  }
])
const state = ref(false);

</script>

<style scoped lang="scss">
@import "../assets/sass/base.scss";

header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  .burger{
    z-index: 3;
    cursor: pointer;
    position: fixed;
    right:50px;
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
  background-color: #5E3AEE;
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

ul{
  position:fixed;
  height:100vh;
  width:100%;
  transform:translate(0%,15%);
  
  li{
  width:100%;
  cursor: pointer;
  text-align: center;
  list-style-type: none;
  padding: 40px 0;
  color: white;
  font-weight: 600;
  font-size: 24px;
  cursor:pointer;
  transition: all 0.5s;
  &:hover{
    font-weight: bold;
  }
  }
}


</style>
