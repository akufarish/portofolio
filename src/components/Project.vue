<template>
  <section id="project" class="bg-white py-20 w-full">
    <div class="">
      <h3 class="text-center text-3xl font-bold font-mono">Project</h3>
      <p class="font-sans text-center text-slate-600">
        Beberapa project yang saya kerjakan
      </p>
    </div>
    <div
      class="grid grid-cols-1 place-items-center lg:grid-cols-2 mt-5 gap-12 mx-12"
    >
      <div v-for="(data, index) in tech" class="group block" :key="index">
        <div
          class="transition-all lg:w-[30vw] flex-col duration-100 bg-white items-center rounded-lg"
        >
          <div class="">
            <div class="flex justify-center items-center relative">
              <img :src="data.img" class="rounded-lg" alt="" />
              <div
                class="absolute z-10 group-hover:z-30 opacity-0 group-hover:opacity-100 rounded-md bg-[#6e6d6d8a] w-full h-full flex justify-center items-center duration-300 transition-opacity"
              >
                <div class="flex">
                  <a :href="data.github" class="font-bold text-4xl"
                    ><i
                      class="bi bi-github text-white hover:text-black transition-colors duration-200"
                    ></i
                  ></a>
                </div>
              </div>
            </div>
            <div class="flex flex-col mt-5 justify-center items-center">
              <h3 class="text-center text-3xl font-bold font-mono">
                {{ data.nama }}
              </h3>
              <p class="font-sans text-center text-slate-600">
                {{ data.deskripsi }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import project1 from "../assets/project1.png";
import project2 from "../assets/project2.png";
import project3 from "../assets/Project.png";
import project4 from "../assets/project4.png";

export default defineComponent({
  data() {
    return {
      tech: [
        {
          img: project1,
          nama: "Tekno",
          deskripsi: "Website untuk mengatur harga dan stok barang",
          github: "https://github.com/akufarish/tekno",

          // width: 120,
        },
        {
          img: project2,
          nama: "Simple cms",
          deskripsi:
            "Website cms (content management system) simple yang dibuat menggunakan vue js dan laravel.",
          github: "https://github.com/akufarish/vue-js-blog",
          // width: 140,
        },
        {
          img: project3,
          nama: "Simulasi MPLS",
          deskripsi:
            "Game bertemakan MPLS yang dibuat untuk mempermudah siswa baru untuk mengenal jurusan.",
          github: "https://github.com/Tefa-PPLG/project-Tefa-B",
          // width: 120,
        },
        {
          img: project4,
          nama: "Shoot rocket",
          deskripsi: "Adalah game bertemakan space shooter dengan style retro.",
          github: "https://github.com/akufarish/project-game",
          // width: 120,
        },
      ],
    };
  },
});
</script>

<style></style>
