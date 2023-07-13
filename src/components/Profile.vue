<template>
  <section id="profile" class="py-20">
    <div class="">
      <h3 class="text-center text-3xl font-bold font-mono">Profile</h3>
      <p class="font-sans text-center text-slate-600">Profile singkat</p>
    </div>
    <div
      class="flex flex-col lg:flex-row gap-12 lg:gap-36 pb-12 justify-center place-items-center mx-12"
    >
      <aside
        class="group flex shadow-lg hover:shadow-md lg:mt-0 mt-12 transition-all duration-150 justify-center items-center relative"
      >
        <img
          src="../assets/farish.jpeg"
          alt=""
          class="max-w-md z-30 rounded-md shadow-lg group-hover:shadow-sm"
          width="220"
        />
        <div
          class="bg-red-600 w-[222px] group-hover:right-4 group-hover:bottom-4 transition-all duration-200 rounded-md h-[293px] z-20 group-hover:bg-red-700 border-[3px] border-red-800 group-hover:border-none right-7 bottom-7 absolute shadow-lg"
        ></div>
        <div
          class="absolute z-10 group-hover:z-30 opacity-0 group-hover:opacity-100 rounded-md bg-[#6e6d6d8a] w-[220px] h-[293px] flex justify-center items-center duration-300 transition-opacity"
        >
          <div class="flex gap-5">
            <a href="https://github.com/akufarish" class="font-bold text-4xl"
              ><i
                class="bi bi-github text-white hover:text-black transition-colors duration-200"
              ></i
            ></a>
            <a
              href="https://www.instagram.com/akuasqolani/"
              class="font-bold text-4xl"
            >
              <i
                class="bi bi-instagram text-white hover:text-black transition-colors duration-200"
              ></i>
            </a>
          </div>
        </div>
      </aside>
      <aside class="w-80">
        <p class="font-medium text-base text-center lg:text-left">
          Halo, nama saya Muhammad Farish Asqalani, biasa dipanggil Farish, saya
          adalah siswa sekolah SMK NEGERI 2 BANJARMASIN, dan saya mengambil
          jurusan PPLG (Perkembangan Perangkat Lunak & Gim). Saya sangat
          tertarik untuk menjelajahi lebih jauh di dunia web development
        </p>
      </aside>
    </div>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({});
</script>

<style></style>
