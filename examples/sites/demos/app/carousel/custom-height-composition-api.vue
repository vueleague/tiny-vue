<template>
  <div>
    <tiny-carousel type="card" height="150px">
      <tiny-carousel-item class="carousel-item-demo" v-for="item in 4" :key="item">
        <h3>{{ item }}</h3>
      </tiny-carousel-item>
    </tiny-carousel>
    <br />
    <tiny-carousel type="card" height="200px">
      <tiny-carousel-item class="carousel-item-demo" v-for="item in 4" :key="item">
        <h3>{{ item }}</h3>
      </tiny-carousel-item>
    </tiny-carousel>
  </div>
</template>

<script setup lang="jsx">
import { Carousel as TinyCarousel, CarouselItem as TinyCarouselItem } from '@opentiny/vue'
</script>

<style scoped>
.block {
  margin: 20px 0;
}

.carousel-item-demo:nth-child(2n) {
  background-color: #99a9bf;
}

.carousel-item-demo:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>
