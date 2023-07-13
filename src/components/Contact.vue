<template>
  <div class="flex justify-center items-center">
    <div
      class="flex p-6 justify-center flex-col max-w-md bg-slate-200 rounded-md shadow-lg"
    >
      <div class="">
        <h3 class="text-3xl font-bold font-mono">Contact</h3>
        <p class="font-sans text-slate-600">
          Beberapa cara untuk menghubungi saya
        </p>
      </div>
      <div v-for="(data, index) in icon" :key="index" class="flex gap-5 mt-5">
        <div class="flex">
          <i
            class="text-black font-bold text-2xl transition-all duration-300"
            :class="data.icons"
          ></i>
        </div>
        <div class="">
          <h3 class="text-xl">{{ data.text }}</h3>
          <h3 class="font-bold text-xl">{{ data.contact }}</h3>
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
          icons: "bi bi-envelope",
          text: "email",
          contact: "risfarishk@gmail.com",
        },
        {
          icons: "bi bi-instagram",
          text: "instagram",
          contact: "@akuasqolani",
        },
      ],
    };
  },
});
</script>

<style></style>
