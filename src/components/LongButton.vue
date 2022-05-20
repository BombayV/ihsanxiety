<script setup>
</script>
<template>
	<button @click="$emit('event')" class="rounded flex justify-start items-center w-full transition duration-150 font-medium hover:shadow-md font-mont m-0.5 hover:bg-gray-600 hover:text-gray-100 hover:border-gray-500 hover:border-b-0 focus:bg-gray-700 focus:text-gray-200 focus:border-gray-500 focus:border-b-0">
		<slot></slot>
	</button>
</template>