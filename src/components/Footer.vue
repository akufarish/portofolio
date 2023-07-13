<template>
  <div class="py-12">
    <div
      class="flex flex-col lg:flex-row gap-5 lg:gap-0 justify-between items-center mx-12"
    >
      <div class="flex">
        <h3 class="font-bold text-xl animate-bounce">Farish</h3>
      </div>
      <div class="flex items-center">
        <ul class="flex gap-5">
          <li class="hover:underline transition-all duration-200">Profile</li>
          <li class="hover:underline transition-all duration-200">
            Tech stack
          </li>
          <li class="hover:underline transition-all duration-200">Project</li>
          <li class="hover:underline transition-all duration-200">Contact</li>
        </ul>
      </div>
      <div class="flex gap-3">
        <div
          v-for="(data, index) in icon"
          :key="index"
          class="bg-gray-400 hover:animate-spin shadow-lg flex justify-center group gap-12 items-center w-full aspect-[3/3] h-12 rounded-full"
        >
          <i
            class="text-white font-bold text-2xl group-hover:text-black transition-all duration-300"
            :class="data.icon"
          ></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  data() {
    return {
      icon: [
        {
          icon: "bi bi-github",
        },
        {
          icon: "bi bi-instagram",
        },
      ],
    };
  },
});
</script>

<style></style>
