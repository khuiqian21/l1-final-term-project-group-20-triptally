<template> 
    <div class="navbar">
  
        <img src="@/assets/triptallylogo.png" class="tt_logo" alt="TripTally">
        <button class="login-button">Login</button>
        <button class="signup-button">Sign Up</button>
  
    </div>
  
</template>
  
<script>
    export default {
        name: 'preNavigationBar',

    }

</script>

<style scoped>
    .navbar {
        display: flex;
        background-color: rgb(72, 159, 181);
        min-height: 10vh;
        align-items: center;
        font-size: calc(5px + 1.5vmin);
    }

    .tt_logo {
        height: 50px;
    }
    
    .login-button, .signup-button {
        padding: 10px 20px;
        font-size: 15px;
        border: none;
        cursor: pointer;
        margin-left: auto;
    }


    .login-button {
        color: white;
        background-color: rgb(72, 159, 181);

    }

    .signup-button {
        background-color: rgb(175,212,219);
        color: #fff;
        margin-left: 5px; 
        border-radius: 20px; 
        margin-right: 20px;
    }

   
</style>