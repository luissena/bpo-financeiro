<template>
  <section class="flex flex-col items-center">
    <h1 class="text-lg font-bold mt-24 pb-2 text-center">
      COM O BPO FINANCEIRO, A SUA EMPRESA:
    </h1>
    <div class="border-t-2 border-[#7D3246] w-[200px]"></div>

    <div>
      <ul
        class="mt-10 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5 justify-center items-center"
      >
        <li
          v-for="item in list"
          class="z-50 px-5 py-5 w-[350px] flex items-center text-center gap-2 bg-[#E4E4E480] rounded-ss-2xl rounded-ee-2xl"
        >
          <IconV />
          <span class="text-lg">{{ item.description }}</span>
        </li>
      </ul>
    </div>
  </section>
</template>

<script setup lang="ts">
type ListProps = {
  description: string
}
const list: ListProps[] = [
  {
    description: "Consegue dar mais foco ao Core Business",
  },
  {
    description: "Recebe informações mais claras, rápidas e efetivas",
  },
  { description: "Tem maior segurança nos dados financeiros" },
  { description: "Tem acesso a especialistas em finanças" },
  { description: "Consegue ter previsibilidade no seu negócio" },
  { description: "Reduz gastos considerados desnecessários" },
]
</script>
