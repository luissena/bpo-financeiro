<template>
  <section class="flex flex-col items-center">
    <h1 class="text-lg font-bold mt-24 pb-2 text-center">
      CLIENTES QUE CONFIAM E INDICAM NOSSA EMPRESA
    </h1>
    <div class="border-t-2 mb-10 border-[#7D3246] w-[200px]"></div>

    <div class="w-4/5 bg-[#E4E4E4] rounded-ss-2xl rounded-ee-2xl">
      <swiper :navigation="true" :modules="modules">
        <swiper-slide>
          <div class="flex items-center py-10 px-20 gap-10">
            <img src="/depoiment.png" />
            <div>
              <h1 class="text-[#7D3246] font-semibold text-lg">
                FULANO DE TAL
              </h1>
              <p class="">
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry. Lorem Ipsum has been the industry's standard dummy
                text ever since the 1500s, when an unknown printer took a galley
                of type and scrambled it to make a type specimen book. It has
                survived not only five centuries, but also the leap into
                electronic typesetting, remaining essentially unchanged. It was
                popularised in the 1960s with the release of Letraset sheets
                containing Lorem Ipsum passages, and more recently with desktop
                publishing software like Aldus PageMaker including versions of
                Lorem Ipsum.
              </p>
            </div>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="flex items-center py-10 px-20 gap-10">
            <img src="/depoiment.png" />
            <div>
              <h1 class="text-[#7D3246] font-semibold text-lg">
                FULANO DE TAL 2
              </h1>
              <p class="">
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry. Lorem Ipsum has been the industry's standard dummy
                text ever since the 1500s, when an unknown printer took a galley
                of type and scrambled it to make a type specimen book. It has
                survived not only five centuries, but also the leap into
                electronic typesetting, remaining essentially unchanged. It was
                popularised in the 1960s with the release of Letraset sheets
                containing Lorem Ipsum passages, and more recently with desktop
                publishing software like Aldus PageMaker including versions of
                Lorem Ipsum.
              </p>
            </div>
          </div>
        </swiper-slide>
      </swiper>
    </div>
  </section>
</template>

<script setup lang="ts">
import { Swiper, SwiperSlide } from "swiper/vue"

// Import Swiper styles
import "swiper/css"

import "swiper/css/navigation"

// import required modules
import { Navigation } from "swiper/modules"

const modules = [Navigation]
</script>

<style>
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-button-prev,
.swiper-button-next {
  color: #7d3246;
}
</style>
