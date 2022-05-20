<script setup>
const reloadPage = () => {
  console.log('reload page')
  window.location.reload()
}
</script>

<template>
  <div style="box-shadow: 0 3px 10px 4px rgb(0 0 0 / 30%)" class="z-40 fixed h-16 w-full bg-green-800 flex justify-between items-center border-b-2 border-b-gray-400">
    <button @click="reloadPage">
      <img class="h-14 ml-2" src="../assets/bulldog.png" alt="Bulldog">
    </button>
    <button @click="$emit('setSidebar')" class="mr-4">
      <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-gray-400 hover:scale-105 duration-200" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
        <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16" />
      </svg>
    </button>
  </div>
</template>