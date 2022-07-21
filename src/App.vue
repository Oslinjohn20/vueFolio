<template>
  <Navbar/>
  <router-view/>
  <FooterCurve class="footer"/>
  
</template>
<script>
import Navbar from "./components/Navbar.vue";
import FooterCurve from "./components/FooterCurve.vue"

export default {
  components: {Navbar, FooterCurve}
}
</script>
<style>
* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  background-image: url(./assets/bg.jpg);
  background-size: cover;
	background-position: bottom; 
	transition: 0.4s;
}
/* .footer {
  display: flex;
  justify-content: center;
  background-color: rgb(129, 120, 120);
} */






</style>
