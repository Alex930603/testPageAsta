<template>

  <div class="flex-column">
    <Navb />
    <Slider />
    <HouseForm />
    <BlogSlide />
  </div>


</template>

<script>

var test = [1, 2, 3, 4]

import Navb from './partials/Navb.vue';
import Slider from './partials/Slider.vue';
import BlogSlide from './partials/BlogSlide.vue';
import HouseFormVue from './HouseForm.vue';



export default {

  name: "FirstPage",

  components: {
    Slider,
    Navb,
    BlogSlide,
    HouseFormVue
  }
}

</script>