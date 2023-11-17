<template>
  <section class="flex flex-col items-center">
    <h1 class="text-lg font-bold mt-24 pb-2 text-center">
      COM O BPO FINANCEIRO, A SUA EMPRESA:
    </h1>
    <div class="border-t-2 border-[#7D3246] w-[200px]"></div>
  </section>

  <ul
    class="grid grid-cols-3 justify-center items-center mx-auto gap-5 w-5/6 text-center py-10"
  >
    <li
      class="bg-[#E4E4E4] text-[#21515D] font-bold rounded-ss-2xl rounded-ee-2xl"
      v-for="item in list"
    >
      <img class="" :src="item.thumbnail" />
      <p class="px-12 py-3">{{ item.description }}</p>
    </li>
  </ul>
</template>

<script setup lang="ts">
type ListProps = {
  description: string
  thumbnail: string
}

const list: ListProps[] = [
  {
    description: "Terá mais tempo para se dedicar em fazer mais dinheiro",
    thumbnail: "/implementation/01.png",
  },
  {
    description: "Terá mais controle do negócio, reduzindo custos",
    thumbnail: "/implementation/02.png",
  },
  {
    description: "Tomará decisões baseadas em métricas precisas",
    thumbnail: "/implementation/03.png",
  },
]
</script>
