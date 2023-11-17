<template>
  <section class="bg-[#F7F7F7] flex flex-col items-center pb-10">
    <img src="/logo.png" />
    <h1 class="text-lg md:w-1/2 text-center">
      Assista ao videdo e descubra como terceirizar o financeiro da sua empresa
      para focar no que realmente importa.
    </h1>

    <div class="py-4 z-50">
      <iframe
        class="p-2 bg-white rounded-lg"
        width="500"
        height="315"
        src="https://www.youtube.com/embed/8vTpJtYGqD8?si=Hynjpbc50g1hWi0S"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        allowfullscreen
      ></iframe>
    </div>

    <h2 class="lg:w-1/3 text-lg text-center">
      Toque no link abaixo e receba um diagnóstico de um
      <span class="font-bold">especialista!</span>
    </h2>

    <button
      class="bg-[#21515D] font-bol w-full md:w-1/2 lg:w-1/4 py-2 rounded-ss-2xl rounded-ee-2xl text-white my-3"
    >
      QUERO CRESCER!
    </button>
    <img class="w-1/4" id="globo" src="/globo.png" />

    <h1 class="text-lg font-bold mt-24 pb-2 text-center">
      SUA EMPRESA JÁ PASSOU OU PASSA POR ALGUMA DESTAS SITUAÇÕES?
    </h1>
    <div class="border-t-2 border-[#7D3246] w-[200px]"></div>

    <div>
      <ul
        class="mt-10 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5 justify-center items-center"
      >
        <li
          v-for="item in list"
          class="px-5 py-5 w-[350px] flex items-center text-center gap-2 bg-[#E4E4E480] rounded-ss-2xl rounded-ee-2xl"
        >
          <IconX />
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
    description: "Comete erros frequentes nos registros financeiros",
  },
  {
    description: "Mistura gastos pessoais com gastos da empresa",
  },
  { description: "Não consegue focar no crescimento do negócio" },
  { description: "Não toma decisões assertivas baseadas em dados concretos" },
  { description: "O negócio tem grande acúmulo de dívidas e não cresce" },
  { description: "Sente dificuldades em realizar boas análises financeiras" },
]
</script>

<style scoped>
#globo {
  position: absolute;
  top: 350px;
  right: 0;

  object-fit: cover;
}
</style>
