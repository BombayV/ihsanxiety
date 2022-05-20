<script setup>
import Navbar from './components/Navbar.vue'
import Intro from './components/Intro.vue'
import Identify from './components/Identify.vue'
import Reduce from './components/Reduce.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <Navbar />
  <Intro />
	<Identify />
	<Reduce />
	<Footer />
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700;800;900&display=swap');

#app {
  margin: 0;
	font-family: "Montserrat", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100vh;

}

/* Scroll Bar */
::-webkit-scrollbar {
	width: 4px;
}

::-webkit-scrollbar-track {
	background-color: #444444;
}

::-webkit-scrollbar-thumb {
	background: #9a9a9a;
}

::-webkit-scrollbar-thumb:hover {
	background: #22381c;
}
</style>
