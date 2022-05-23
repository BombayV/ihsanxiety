<script setup>
const scrollTo = (to, duration) => {
	console.log('test')
	if (duration <= 0) return;
	const element = document.getElementById('btn');
	const difference = to - element.scrollTop;
	const perTick = difference / duration * 10;

	setTimeout(function() {
		element.scrollTop = element.scrollTop + perTick;
		if (element.scrollTop === to) return;
		scrollTo(element, to, duration - 10);
	}, 10);
}
</script>

<template>
  <div class="grad h-screen relative flex flex-col items-center justify-center z-10">
		<h1 style="animation: fade 2s" class="mb-2 text-3xl lg:text-7xl font-bold text-gray-50 text-center drop-shadow-2xl">Feeling overwhelmed?</h1>
		<p style="animation: fadeIn 2s" class="lg:text-2xl font-mont text-center mr-4 ml-4 lg:mr-12 lg:ml-12 font-medium text-gray-300 transition duration-500">This could be a sign of anxiety. Press the button below to keep reading more about it.</p>
		<button style="animation: fadeBottom 2s" class="lg:pt-2 lg:pb-2 pb-1.5 pt-1.5 bg-green-500 hover:bg-green-400 duration-500 lg:text-xl transition rounded-md font-semibold text-gray-900 text-sm mt-6 shadow-md border-none animate-bounce"><a class="w-full h-full lg:pr-10 lg:pl-10 lg:pt-2 lg:pb-2 pb-1.5 pt-1.5 pl-5 pr-5" href="#intro">Learn more about anxiety!</a></button>
  </div>
	<div id="intro" class="h-screen grad-wavy bg-green-700 flex items-center justify-center flex-col">
		<h2 class="mb-2 text-3xl lg:text-7xl font-bold text-gray-50 text-center drop-shadow-xl">What is anxiety?</h2>
		<p class="text-center lg:text-2xl 2xl:text-3xl font-mont text-center mr-4 ml-4 lg:mr-12 lg:ml-12 font-medium text-neutral-300 transition duration-500 mt-4 drop-shadow-md">
			Anxiety is our body's reaction to dangerous or stressful situations. While many people see it as a negative emotion, it actually is a positive emotion in many ways as it
			engages our body's natural alarm system when we are in a situation where we may be at risk or danger. Anxiety can be a symptom of many different things, but it is usually
			related to a situation that we are in. It is a way to understand how we feel about the things that are happening to us and how we can deal with them.
		</p>
		<p class="text-center lg:text-2xl 2xl:text-3xl font-mont text-center mr-4 ml-4 lg:mr-12 lg:ml-12 font-medium text-neutral-300 transition duration-500 mt-4 drop-shadow-md">
			However, it is important to understand the difference between anxiety and having an anxiety disorder. Anxiety disorders are more serious and can affect our health.
			Unlike anxiety, anxiety disorders are persistent and excessive thoughts/worries that do not go away easily, even if there's nothing to be stressed about. It is important to identify
			our own anxiety in order to better understand how we can deal with it.
		</p>
		<svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 lg:w-20 lg:h-20 text-gray-300 animate-bounce mt-8 lg:mt-8 opacity-80" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
			<path stroke-linecap="round" stroke-linejoin="round" d="M19 13l-7 7-7-7m14-8l-7 7-7-7" />
		</svg>
	</div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700;800;900&display=swap');

.grad {
	background-image: url("../assets/blob.svg");
	background-repeat: repeat;
	background-size: cover;
	background-position: center;
} /* 15803D, 16A34A, 59fa3c */

.grad-wavy {
	background-image: url("../assets/wavy.svg");
	background-repeat: repeat;
	background-size: cover;
	background-position: center;
}

.grad-wave {
	background-image: url("../assets/wave.svg");
	background-repeat: repeat;
	background-size: cover;
	background-position: center;
}

.grad-stacked {
	background-image: url("../assets/stacked.svg");
	background-repeat: repeat;
	background-size: cover;
	background-position: center;
}

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