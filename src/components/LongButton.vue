<script setup>
</script>
<template>
	<button @click="$emit('event')" class="rounded flex justify-start items-center w-full transition duration-150 font-medium hover:shadow-md font-mont m-0.5 hover:bg-neutral-600 hover:text-neutral-100 hover:border-neutral-500 hover:border-b-0 focus:bg-neutral-700 focus:text-neutral-200 focus:border-neutral-500 focus:border-b-0">
		<slot></slot>
	</button>
</template>