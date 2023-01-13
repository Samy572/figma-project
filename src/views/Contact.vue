<script setup lang="ts">

</script>
<template>
    <div id="contact">
        <h2>Contact</h2>
        <div class="containerPlane">
            <img src="../assets/images/hshs 1.svg" alt="Paper plane"/>
        </div>
        <form>
             <label for="name" >Name</label>
              <input type="text" id="name">
              <label for="email" >Email</label>
              <input type="text" id="email">
              <label for="message">Message</label>
              <textarea name="message" id="message" cols="20" rows="10"></textarea>
        <button type="submit">Submit</button>
        </form>
        <footer>

            <p>@reboot13_dev</p>

        </footer>
  </div>

</template>



<style scoped lang="scss">

#contact{
    position: relative;
    min-height:100vh;
    width:100%;
    background-color: #5E3AEE;
    h2{
        padding-top: 50px;
        color:white;
        font-size: 33px;
        font-weight: 800;
        text-align: center;
    }
}

.containerPlane{
    padding-top: 50px;
    width:100%;
    height: auto;
    display: flex;
    justify-content: center;

    img{
        width:240px;
        height:124px;
    }
}
form{
    max-width: 450px;
    display: flex;
    flex-direction: column;
    margin: 0 auto;
    padding: 10px 30px 100px 30px;

    label{
        color:white;
        font-size: 12px;
        padding: 5px 0;
       
    }
    button{
        margin-top: 25px;
        height: 34px;
        cursor: pointer;
    }
}

footer{
   position: absolute;
   bottom: 0;
   display: flex;
   align-items: center;
   justify-content: center;
    width:100%;
    height:53px;
    background-color:#BFB8B8;
 
}
p{
       
        font-size:16px;
        color:#696969;
        font-weight:500;
    }
</style>
