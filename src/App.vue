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
#app {
  margin: 0;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen',
  'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue',
  sans-serif;
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
