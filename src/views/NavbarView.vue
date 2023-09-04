<script setup lang="ts">

</script>

<template>
  <nav class="navbar">

    <div class="logo">
      <img src="https://w7.pngwing.com/pngs/635/870/png-transparent-logo-flower-flower-purple-violet-logo-thumbnail.png" alt="logo">
    </div>
    
    <ul class="nav-links">
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Works</a></li>
      <li><a href="#">Contact</a></li>
    </ul>

  </nav>
</template>

<style scoped>

.navbar{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  width: 100%;
  background-color: #000;
  padding: 0rem 10rem;

}

/* .navbar>.logo{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  height: 100vh;
  width: 100vw;
  background-color: #000;
} */
.navbar>.logo>img{
 width: 100px;
  height: 100px;
  border-radius: 50%;
  object-fit: cover;
}

.navbar>.nav-links{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-around;
  /* height: 100vh;
  width: 100vw; */
  width: 100%;
  background-color: #000;
   padding: 0rem 10rem;
}
.navbar>.nav-links>li{
  list-style: none;
  padding: 0rem 2rem;
}
  
</style>