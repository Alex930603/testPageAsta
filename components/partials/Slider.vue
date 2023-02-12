<template>
  <Carousel>
    <Slide v-for="slide in 10" :key="slide">
      <div class="carousel__item">{{ slide }}</div>
    </Slide>

    <template #addons>
      <Navigation />
      <Pagination />
    </template>
  </Carousel>
</template>

<script>


import { defineComponent } from 'vue'
import { Carousel, Navigation, Pagination, Slide } from 'vue3-carousel'
import axios from "axios"
import './../../node_modules/vue3-carousel/dist/carousel.css'



export default defineComponent({
  name: 'Slider',
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
})
/* 
var immagini = []


const getHouseImages = async () => {
  const response = await axios.get('https://picsum.photos/200/300', {
    params: {
      query: 'house',
      count: 10,
    }
  });
  return console.log(response.data)

};

console.log(respomse)
 */
</script>

<style>
.carousel__item {
  min-height: 200px;
  width: 100%;
  background-color: #ad1919;
  color: #ffffff;
  font-size: 20px;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.carousel__slide {
  padding: 10px;
}

.carousel__prev,
.carousel__next {
  box-sizing: content-box;

}
</style>