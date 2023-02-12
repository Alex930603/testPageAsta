<script>

import { defineComponent } from 'vue'
import Bottone from './Bottone.vue';
import Slider from "./Slider.vue"
import './../../node_modules/vue3-carousel/dist/carousel.css'

export default {


  name: "BlogSlide",


  components: {
    Bottone,
    Slider
  }

}
</script>


<template>

  <div class="flex justify-center">
    <div class="w-9/12 text-center">
      <h1 class="font-medium">I nostri ultimi articoli Blog</h1>

      <div>
        <Slider />
      </div>

      <Bottone functionality="Cerca" bgColor="bg-blue-500" />
    </div>
  </div>
</template>


<style>

</style>
