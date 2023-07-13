<template>
  <nav class="bg-violet-600 text-slate-200 p-4 font-sans">
    <ul class="flex justify-between items-center mx-3 lg:mx-12">
      <li class="text-white text-xl font-sans font-medium">FARISH</li>
      <div class="gap-12 hidden lg:flex">
        <li class="hover:text-white hover:font-medium transition-all">
          <a href="#profile">Profile</a>
        </li>
        <li class="hover:text-white hover:font-medium transition-all">
          <a href="#skill">Tech stack</a>
        </li>
        <li class="hover:text-white hover:font-medium transition-all">
          <a href="#project">Project</a>
        </li>
        <li
          class="hover:text-white font-bold font-mono hover:font-medium transition-all"
        >
          <a href="#">Contact</a>
        </li>
      </div>
      <li>
        <button
          class="px-6 py-2 hidden lg:block border-2 text-yellow-200 rounded-full border-yellow-300 hover:bg-yellow-300 hover:text-black transition-all"
        >
          Contact
        </button>
      </li>
      <button @click="responsive" class="flex lg:hidden flex-col gap-1">
        <div class="bg-white h-2 w-2 rounded-full"></div>
        <div class="bg-white h-2 w-2 rounded-full"></div>
        <div class="bg-white h-2 w-2 rounded-full"></div>
      </button>
    </ul>
  </nav>
  <div class="flex justify-end">
    <div
      v-if="isShow == true"
      class="bg-white absolute flex mr-4 justify-center items-center rounded-lg w-32 aspect-[2/3] shadow-md"
    >
      <ul>
        <li class="text-black text-lg font-medium">
          <a href="#">Profile</a>
        </li>
        <li class="text-black text-lg font-medium">
          <a href="#">Tech stack</a>
        </li>
        <li class="text-black text-lg font-medium">
          <a href="#">Project</a>
        </li>
        <li class="text-black text-lg font-medium">
          <a href="#">Contact</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, onMounted } from "vue";

export default defineComponent({
  data() {
    return {
      isShow: false,
    };
  },

  methods: {
    responsive() {
      this.isShow = !this.isShow;
    },
  },
});
</script>

<style></style>
