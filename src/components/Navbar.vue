<template>
  <nav>
    <img src="../assets/mylogo.png" alt="Oslin">
    <div >
        <router-link to="/about">About</router-link>  
        <router-link to="/contact">Contact</router-link>   
        <router-link to="projects">Projects</router-link>  
        <router-link to="testimonials">Testimonials</router-link>   
        <router-link to="/">Home</router-link> 
 
    </div>

  </nav>
</template>

<script>
export default {

}
</script>

<style>
nav { 
  top: 0;
  z-index: 9999;
  padding: 5px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: rgb(129, 120, 120);;
}

nav img {
    height: 76px;
    display: table;
    text-align: left; 
    border-radius: 50%; 
}

nav a {
  font-weight: bold;
  color: #2c3e50;
  padding: 10px;
  text-decoration: none;
  
  
}

nav a.router-link-exact-active {
   color: #fff;
  text-shadow:
      0 0 7px #fff,
      0 0 10px #fff,
      0 0 21px #fff,
      0 0 42px #0fa,
      0 0 82px #0fa,
      0 0 92px #0fa,
      0 0 102px #0fa,
      0 0 151px #0fa;
}
</style>