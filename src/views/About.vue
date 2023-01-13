<template>
  <div class="about">
    <div class="bloc"></div>

    <h2>A Bit About Me...</h2>
    <p>Hello, My name is Krutik Raut AKA <br />reboot13.</p>
    <p>I am a CSE Undergraduate at <br />Paul University.</p>
    <p>
      I'm currently learning UI/UX developpment. Checkout my projects on github. <br />
      <span>@reboot13-git</span>
    </p>

    <div class="containerPhone">
      <img src="../assets/images/Mockup@2x.svg" alt="smartphone" />
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped lang="scss">
.about {
  height: 100vh;
  width: 100%;
  background-color: #0f1221;
  display: block;
  text-align: center;
  color: white;
  h2 {
    font-size: 32px;
    line-height: 48px;
    padding: 50px 0;
    font-weight: 700;
    margin-bottom: 12px;
  }
  p {
    font-size: 18px;
    line-height: 30px;
    font-weight: 500;
    span {
      color: #5e3aee;
    }
  }
}

.bloc {
  margin: 0px auto 0 auto;
  transform: translateY(20px);

  width: 186px;
  height: 21px;
  background-color: #5e3aee;
  justify-content: center;
}

.containerPhone {
  height: 256px;
  
}
</style>
