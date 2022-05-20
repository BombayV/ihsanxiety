<script setup></script>

<template>
  <div class="bg-green-700 h-[49em] relative flex flex-col items-center justify-center z-10">
		<h1 style="animation: fade 2s" class="mb-2 text-3xl lg:text-6xl font-bold text-gray-50 text-center">Feeling overwhelmed?</h1>
		<p style="animation: fadeIn 2s" class="lg:text-xl font-mont text-center mr-4 ml-4 font-medium text-gray-300 transition duration-500">This could be a sign of anxiety. Press the button below to keep reading more about it.</p>
		<button style="animation: fadeBottom 2s" class="lg:pr-10 lg:pl-10 lg:pt-2 lg:pb-2 pb-1.5 pt-1.5 pl-5 pr-5 bg-green-500 hover:bg-green-400 duration-500 lg:text-lg transition rounded-md font-semibold text-gray-900 text-sm mt-6 shadow-md border-none animate-bounce">Learn more about anxiety!</button>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700;800;900&display=swap');

@keyframes fade {
	0% {
		opacity: 0;
		transform: translateY(-50px);
	}
	100% {
		opacity: 1;
		transform: translateY(0px);
	}
}

@keyframes fadeBottom {
	0% {
		opacity: 0;
		transform: translateY(50px);
	}
	100% {
		opacity: 1;
		transform: translateY(0px);
	}
}

@keyframes fadeIn {
	0% {
		opacity: 0;
	}
	100% {
		opacity: 1;
	}
}

</style>