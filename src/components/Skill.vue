<template>
  <div class="bg-gray-200 py-20 w-full">
    <div class="">
      <h3 class="text-center text-3xl font-bold font-mono">Tech stack</h3>
      <p class="font-sans text-center text-slate-600">
        Tech stack yang saya gunakan
      </p>
    </div>
    <div class="grid grid-cols-2 lg:grid-cols-3 mt-5 gap-12 mx-12">
      <div v-for="(data, index) in tech" class="group" :key="index">
        <div
          class="flex justify-center transition-all duration-300 bg-slate-100 items-center group-hover:bg-white grayscale group-hover:grayscale-0 py-6 h-52 lg:px-7 px-2 rounded-lg shadow-xl"
        >
          <img :src="data.img" :width="data.width" class="" alt="" />
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
      tech: [
        {
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/2048px-HTML5_logo_and_wordmark.svg.png",
          width: 120,
        },
        {
          img: "https://www.freepnglogos.com/uploads/html5-logo-png/html5-logo-css-logo-png-transparent-svg-vector-bie-supply-9.png",
          width: 140,
        },
        {
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/JavaScript-logo.png/800px-JavaScript-logo.png",
          width: 120,
        },
        {
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Typescript_logo_2020.svg/2048px-Typescript_logo_2020.svg.png",
          width: 120,
        },
        {
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/2/27/PHP-logo.svg/2560px-PHP-logo.svg.png",
          width: 220,
        },
        {
          img: "https://logospng.org/download/laravel/logo-laravel-1024.png",
          width: 320,
        },
        {
          img: "https://cdn.icon-icons.com/icons2/2699/PNG/512/vuejs_logo_icon_169247.png",
          width: 220,
        },
        {
          img: "https://www.matawebsite.com/images/blog/375_sveltejs_ramping_dan_elegan.png",
          width: 220,
        },
        {
          img: "https://cdn.icon-icons.com/icons2/2699/PNG/512/tailwindcss_logo_icon_170649.png",
          width: 320,
        },
      ],
    };
  },
});
</script>

<style></style>
