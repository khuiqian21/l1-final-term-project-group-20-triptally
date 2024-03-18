<template> 
  <div class="navbar">

    <img src="@/assets/triptallylogo.png" class="tt_logo" alt="TripTally">
    

      <img src="@/assets/home.png" class="home_logo" alt="Home">


      <div class="username" v-if="userName"> {{ userName }} </div>
      <div class="profile" v-if="userName">
        <div class="profile-placeholder"> {{ generateInitials(userName) }} </div>
      </div>


  </div>

</template>

<script>
export default {
  name: 'NavigationBar',
  data() {
    return {
      userName: 'Vanessa Koh'
    };
  },

  methods: {
    generateInitials(name){
      const words = name.split(' ');
      return words.map(word => word.charAt(0)).join('');
    }
  }
}

</script>

<style scoped>


.navbar {
  display: flex;
  background-color: rgb(72, 159, 181);
  min-height: 10vh;
  align-items: center;
  font-size: calc(5px + 1.5vmin);
  width: 100%; 
}

.left {
  margin-left: auto;
}
.tt_logo {
  height: 50px;
  
}
.home_logo {
  height: 30px;
  margin-left: auto;

}
.username {
  color: white;
  margin-left: auto;
}

.profile {
  width: 60px; 
  height: 60px; 
  border-radius: 50%;
  background-color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 20px;
  margin-right: 20px;
  order: 3;
}

.profile-placeholder {
  font-size: 20px;
  color: rgb(72, 159, 181);
  text-transform: uppercase;
}
</style>