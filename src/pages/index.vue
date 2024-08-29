<script setup>
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'
import slide1 from '@/assets/gss-slide.jpg';
import slide2 from '@/assets/slide4.jpg';
import slide3 from '@/assets/slide3.jpg';

const slides = ref([slide1, slide2, slide3])
useHead({
	title: 'GSS Girls PG College, Chirawa',
});
</script>

<template>
	<AppHeader />
	<div class="max-w-7xl mx-auto p-0 m-0">
	<carousel ::autoplay="500" :wrap-around="true">
    <slide v-for="(sl, i) in slides" :key="i">
		<div class="carousel__item"><img :src="sl" class="object-cover h-full w-full" /></div>
    </slide>

    <template #addons>
      <navigation />
    </template>
  </carousel>
</div>
	<Footer />
</template>

<style>
.carousel__item {
  min-height: 200px;
  width: 100%;
  background-color: var(--vc-clr-secondary)ß;
  color: var(--vc-clr-white);
  font-size: 20px;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.carousel__slide {
  padding: 0;
  margin: 0;
  width: 100%;
}

.carousel__prev,
.carousel__next {
  box-sizing: content-box;
  border: 1px solid white;
}
</style>

<route lang="yaml">
name: home
</route>
