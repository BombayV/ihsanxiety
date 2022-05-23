<script setup>
import {defineProps} from 'vue'
defineProps({
	title: {
		type: String,
		default: 'Test anxiety',
	},
	description: {
		type: String,
		default: 'Some description goes here that can be used to describe the anxiety. This can be a long description that can be used to describe the anxiety.',
	},
})
</script>

<template>
	<div class="relative w-3/4 lg:w-2/5 xl:w-1/4 h-44 mt-4 ml-4 mr-4 mb-4 bg-neutral-800 flex items-start justify-start rounded-xl shadow-lg">
		<div class="w-1/5 h-full ml-3 mt-3">
			<span class="w-12 h-12 bg-green-500 rounded-lg flex justify-center items-center">
				<slot></slot>
			</span>
		</div>
		<div class="w-4/5 h-full flex flex-col items-start justify-evenly">
			<h2 class="text-lg font-medium text-neutral-200 text-center drop-shadow-xl capitalize lg:mt-2">{{title}}</h2>
			<span class="text-left text-md text-neutral-400 transition duration-500 drop-shadow-md lg:mb-2 mr-4">
				{{description}}
			</span>
		</div>
	</div>
</template>