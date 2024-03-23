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
      <AppCat/>
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
</script>
