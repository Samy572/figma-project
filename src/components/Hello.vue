<template>
<section id="hello">

<div class="home">
    <h1 class="title">Hello, <br> I am <span>Krutik Raut.</span></h1>
    <h2>Web Designer/Developer</h2>
    <p class="description">I sepcialise in UI Design, Responsive Web Design, <br>and Web development.</p>
  

    <div class="buttonContainer">
        <button class="btn contact">Contact</button>
        <button class="btn project">Projects</button>
    </div>
    <div class="laptop">
     <img src="../assets/images/laptop 1.png" alt="laptop">
     
    </div>
</div>
</section>


</template>

<script setup lang ="ts">
import { ref } from '@vue/reactivity';


</script>

<style scoped lang="scss">


#hello{
    text-align: center;
    width:100%;
    display: flex;
    justify-content: center;
    margin: 33px 0 33px 0;
   
}

.home{
    display: flex;
    flex-direction: column;
    height:468px;
    width:309px;
    background-color:#F0F0F5 ;
}
.title{
padding-top: 34px;
}
span{
    color:#5E3AEE;
}
h2{
    margin-top: 10px;
    color:#696969;
    font-size: 14px;
}
.description{
    margin-top: 5px;
    font-size: 10px;
    color:black;
}
.buttonContainer{
    margin-top: 25px;
    display: flex;
    flex-direction: column;
    align-items: center;
    .btn{
    height:32px;
    width:131px;
    box-shadow: -4px 5px 4px rgba(0, 0, 0, 0.25);
    border: none;
    cursor: pointer;
}
}
.contact{
        background-color: #ffff;
        margin-bottom: 12px;
    }
    .project{
        color:#fff;
        background-color: #5E3AEE;
        margin-bottom: 17px;
    }
.laptop{
    display: flex;
    justify-content: center;
    
    img{
        width:209px;
        height: 190px;
    }
}


</style>