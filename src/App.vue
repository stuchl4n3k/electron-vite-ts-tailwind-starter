<template>
  <div class="h-screen w-screen flex flex-col pt-12">
    <TopBar />
    <HelloWorld msg="Hello Electron + Vite + Tailwind + TypeScript" />
    <!-- [ HERE COMES YOUR CONTENT ] -->
    <transition name="fade" appear>
      <div class="flex flex-col items-center justify-center h-full pb-0">
        <img class="h-48 ml-5" src="/logo.png" draggable="false" />
      </div>
    </transition>
  </div>
</template>

<script lang="ts">
import TopBar from './components/layout/TopBar.vue'
import HelloWorld from './components/HelloWorld.vue'

import { defineComponent } from 'vue'
export default defineComponent({
  name: 'App',
  components: {
    TopBar,
    HelloWorld,
  },
});
</script>
