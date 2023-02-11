<template>

  <div class="flex-column">
    <Navb />
    <Carousel />
  </div>


</template>

<script>

var test = [1, 2, 3, 4]

import Navb from './partials/Navb.vue';
import Carousel from './partials/Carousel.vue';


export default {

  name: "FirstPage",

  components: {

    Carousel,
    Navb

  }
}

</script>