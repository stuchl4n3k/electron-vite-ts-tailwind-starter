<template>
  <div class="mx-3 text-center">
    <h1 class="text-xl my-5 text-center">{{ msg }}</h1>

    <p class="text-sm text-center my-5">
      <a href="https://vitejs.dev/guide/features.html" target="_blank">Vite Docs</a> |
      <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Docs</a>
    </p>

    <button @click="count++" class="bg-gray-300 hover:bg-gray-400 text-gray-800 font-bold py-2 px-4 rounded inline-flex items-center">
      <svg class="fill-current w-4 h-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20">
        <path d="M13 8V2H7v6H2l8 8 8-8h-5zM0 18h20v2H0v-2z"/>
      </svg>
      <span>Download (count {{ count }})</span>
    </button>

    <p class="text-center my-5">
      Edit <code class="px-2 py-1 bg-gray-700 text-gray-300">components/HelloWorld.vue</code> to test hot reload.
    </p>
  </div>
</template>

<script lang="ts">
  import {defineComponent, ref} from 'vue'

  export default defineComponent({
    name: 'HelloWorld',
    props: {
      msg: {
        type: String,
        required: true
      }
    },
    setup: () => {
      const count = ref(0)
      return {count}
    }
  })
</script>
