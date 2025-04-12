<script>
export default {
  name: 'Header',

  data() {
    return {
      categoriesMenu: [{ name: 'Europa' }, { name: 'Asia' }, { name: 'Indonesia' }],
    }
  },
}
</script>

<template>
  <div class="flex flex-row items-center mx-auto w-full justify-between">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      fill="none"
      viewBox="0 0 24 24"
      stroke-width="1.5"
      stroke="currentColor"
      class="size-6"
    >
      <path
        stroke-linecap="round"
        stroke-linejoin="round"
        d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z"
      />
    </svg>
    <div class="flex flex-row items-center gap-4">
      <div v-for="menu in categoriesMenu" :key="menu">{{ menu.name }}</div>
    </div>
    <div class="flex flex-row">
      <div class="bg-gray-200 rounded-lg px-4 py-1">subcriptions</div>
      <div class="bg-gray-200 ml-4 rounded-lg px-4 py-1">login</div>
    </div>
  </div>
</template>
