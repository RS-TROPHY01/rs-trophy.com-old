<template>
      <div class="mx-auto">
        <div v-for="(product, index) in products" :key="index">
          <h2 class="text-center">ถ้วยรางวัลรหัส {{ product.name }}</h2>
          <div
            class="gap-2 grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5"
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
</template>

<script setup lang="ts">
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
