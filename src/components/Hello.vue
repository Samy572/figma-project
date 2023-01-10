<template>
<section id="hello">

<div class="home">
<h1 class="title">Hello, <br> I am <span>Krutik Raut.</span></h1>
<h2>Web Designer/Developer</h2>
<p class="description">I sepcialise in UI Design, Responsive Web Design, <br>and Web development.</p>
  <div class="btn"></div>
</div>


</section>


</template>

<script setup lang ="ts">

</script>

<style scoped lang="scss">


#hello{
    text-align: center;
    height:468px;
    max-width: 100%;
    display: flex;
    flex-direction: column;
    margin: 33px;
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
</style>