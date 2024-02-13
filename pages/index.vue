<template>
  <AppHeroSection />
  <div class="mx-auto items-center gap-x-8 gap-y-16 p-2 lg:px-8">
    <div class="mx-auto max-w-4xl">
      <h2 class="text-3xl text-gray-900 sm:text-4xl mx-auto">
        RS TROPHY ถ้วยรางวัลคุณภาพดี
      </h2>
      <p class="mt-4 text-gray-500 mx-auto">
        RS TROPHY บริษัทจัดจำหน่ายถ้วยรางวัลคุณภาพดีแข็งแรงทนทาน
        พร้อมมีทีมกราฟิกดีไซน์บริการการออกแบบฟรี
        โดยเรามีทั้งในรูปแบบหน้าร้านและออนไลน์พร้อมบริการจัดส่งทั่วประเทศไทย
      </p>
    </div>
    <div class="py-4">
      <h1 class="text-center">ถ้วยรางวัล</h1>
      <div class="mx-auto">
        <div v-for="(product, index) in products" :key="index">
          <h2 class="text-center">ถ้วยรางวัลรหัส {{ product.name }}</h2>
          <div
            class="gap-2 grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 2xl:grid-cols-6"
          >
            <img
              v-for="index in product.photo"
              :key="index"
              :src="`/catalog/${product.name}/${index}.jpg`"
              width="295px"
              height="295px"
              loading="lazy"
              alt="ผลงานถ้วยรางวัลที่ผ่านมา"
              title="ผลงานถ้วยรางวัลที่ผ่านมา"
              aria-label="ผลงานถ้วยรางวัลที่ผ่านมา"
              class="scaleup"
            />
          </div>
        </div>
      </div>
      <AppOurCustomer />
    </div>
  </div>
</template>
<script setup lang="ts">
const title = "RS TROPHY | ถ้วยรางวัล คุณภาพดีแข็งแรงทนทาน";
const description =
  "บริษัทจัดจำหน่ายถ้วยรางวัลคุณภาพดีแข็งแรงทนทาน โดยเรามีทั้งในรูปแบบหน้าร้านและออนไลน์พร้อมบริการจัดส่งทั่วประเทศไทย";
const image = "/panel/hero_section.webp";
useSeoMeta({
  title: title,
  ogTitle: title,
  twitterTitle: title,
  description: description,
  ogDescription: description,
  twitterDescription: description,
  ogImage: image,
  twitterImage: image,
  keywords: "RS TROPHY, ถ้วยรางวัล",
});
const products = [
  {
    photo: 29,
    name: "B",
  },
  {
    photo: 3,
    name: "T",
  },
  {
    photo: 2,
    name: "FOOTBALL",
  },
  {
    photo: 12,
    name: "D",
  },
  {
    photo: 3,
    name: "L",
  },
  {
    photo: 2,
    name: "LP",
  },
  {
    photo: 36,
    name: "IT-1",
  },
  {
    photo: 12,
    name: "IT-2",
  },
  {
    photo: 6,
    name: "IT-4",
  },
  {
    photo: 6,
    name: "IT-5",
  },
];
</script>
