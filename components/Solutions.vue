<template>
  <section class="flex flex-col items-center">
    <img class="w-1/4" id="globo" src="/globo.png" />

    <h1 class="text-lg font-bold mt-24 pb-2 text-center">
      CONHEÇA NOSSAS SOLUÇÕES
    </h1>
    <div class="border-t-2 border-[#7D3246] w-[200px]"></div>
    <img class="w-1/2 py-16" src="/solutions.png" />
    <img class="w-1/4" id="globo_left" src="/globo_left.png" />
  </section>
</template>

<style scoped>
#globo {
  position: absolute;
  top: 2700px;
  right: 0;

  object-fit: cover;
}
#globo_left {
  position: absolute;
  top: 3800px;
  left: 0;

  object-fit: cover;
}
</style>
