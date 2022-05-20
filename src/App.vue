<script setup>
import Navbar from './components/Navbar.vue'
import Intro from './components/Intro.vue'
import Identify from './components/Identify.vue'
import Reduce from './components/Reduce.vue';
import Footer from './components/Footer.vue';
import LongButton from './components/LongButton.vue';
import {ref} from "vue";

const sidebarState = ref(false)
const setSidebar = (bool) => {
	console.log(bool)
	sidebarState.value = bool
}
</script>

<template>
	<transition name="slide-fade">
		<div v-show="sidebarState" class="fixed z-50 flex justify-center items-center w-full h-48 mt-4">
			<div class="w-full pl-3 pr-3 pt-4 pb-4 bg-gray-300 rounded-lg mr-2.5 ml-2.5 shadow-md">
				<div class="w-full flex justify-between items-center mb-2">
					<span class="text-zn-100 font-semibold font-mont text-md ml-3">IHS Anxiety Project</span>
					<button @click="setSidebar(false)" class="focus:ring-3 focus:ring-green-500 flex items-center justify-center mr-3 transition duration-150 rounded bg-gray-600 hover:bg-gray-500 w-9 h-9">
						<svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
							<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
						</svg>
					</button>
				</div>
				<LongButton class="text-gray-800 pl-3 pr-3 pt-1.5 pb-1.5">
					What is anxiety ?
				</LongButton>
				<LongButton class="text-gray-800 pl-3 pr-3 pt-1.5 pb-1.5">
					Identify anxiety
				</LongButton>
				<LongButton class="text-gray-800 pl-3 pr-3 pt-1.5 pb-1.5">
					Reduce anxiety
				</LongButton>
			</div>
		</div>
	</transition>
	<Navbar @setSidebar="setSidebar(true)"/>
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

.slide-fade-enter-active,
.slide-fade-leave-active{
	transition: all 0.3s ease-out;
}
.slide-fade-enter-from,
.slide-fade-leave-to {
	transform: translateY(-150px);
	opacity: 0;
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
