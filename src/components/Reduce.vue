<script setup>
import Block from './Block.vue'
</script>

<template>
	<div id="reduce" class="pt-8 grad-stacked bg-green-700 flex items-center justify-center flex-col">
		<h2 class="mb-2 mt-16 text-3xl lg:text-7xl font-bold text-gray-50 text-center drop-shadow-xl">Reduce anxiety</h2>
		<p class="text-center lg:text-2xl 2xl:text-3xl font-mont text-center mb-4 mr-4 ml-4 lg:mr-12 lg:ml-12 font-medium text-gray-300 transition duration-500 mt-4 drop-shadow-md">
			It is important to understand that not all the following methods may help you reduce anxiety; however, they are the most common methods that are used to reduce anxiety.
		</p>
		<div class="flex flex-col lg:flex-row lg:justify-evenly flex-wrap items-center justify-center w-full mb-16">
			<Block title="Get Help" description="Don't be hesitant to ask for help. Just like many health conditions, anxiety is more difficult to treat over time.">
				<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-neutral-900" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
					<path stroke-linecap="round" stroke-linejoin="round" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
				</svg>
			</Block>
			<Block title="Avoid alcohol and drugs" description="Alcohol and drug can cause and worsen anxiety. If you have an addiction to any substance, ask for professional advice.">
				<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-neutral-900" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
					<path stroke-linecap="round" stroke-linejoin="round" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z" />
				</svg>
			</Block>
			<Block title="Deep breathing" description="During moments of anxiety, you may only need a small deep breathing session. Take a couple of deep breaths and empty your mind.">
				<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-neutral-900" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
					<path stroke-linecap="round" stroke-linejoin="round" d="M3 15a4 4 0 004 4h9a5 5 0 10-.1-9.999 5.002 5.002 0 10-9.78 2.096A4.001 4.001 0 003 15z" />
				</svg>
			</Block>
			<Block title="Stay active" description="Doing 30 minutes of exercise or participating in activities you enjoy can make you feel good about yourself. Enjoy the moment.">
				<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-neutral-900" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
					<path stroke-linecap="round" stroke-linejoin="round" d="M17.657 18.657A8 8 0 016.343 7.343S7 9 9 10c0-2 .5-5 2.986-7C14 5 16.09 5.777 17.656 7.343A7.975 7.975 0 0120 13a7.975 7.975 0 01-2.343 5.657z" />
					<path stroke-linecap="round" stroke-linejoin="round" d="M9.879 16.121A3 3 0 1012.015 11L11 14H9c0 .768.293 1.536.879 2.121z" />
				</svg>
			</Block>
			<Block title="Minimize phone use" description="Waiting for a message or checking the time can lead to anxiety. Put your phone aside while you sleep and when going outside.">
				<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-neutral-900" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
					<path stroke-linecap="round" stroke-linejoin="round" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z" />
				</svg>
			</Block>
			<Block title="Practice self-care" description="Take some time for yourself. Reading a book, practicing a hobby, or stretching before bed are simple ways to reduce stress.">
				<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-neutral-900" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
					<path stroke-linecap="round" stroke-linejoin="round" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z" />
				</svg>
			</Block>
		</div>
	</div>
</template>