<script setup>
	import maa from '@/assets/maa-gss.jpg';
	import slide from '@/assets/gss-slide.jpg';
	import slide2 from '@/assets/slide4.jpg';
	import slide3 from '@/assets/slide3.jpg';
	useHead({
		title: 'GSS Girls PG College, Chirawa',
	});
	onMounted(async () => {
		const { Carousel, initTWE } = await import("tw-elements");
		initTWE({ Carousel });
		});
</script>

<template>
	<AppHeader />
	<div
		id="carouselExampleCaptions"
		class="relative max-w-7xl mx-auto h-[700px]"
		data-twe-carousel-init
		data-twe-ride="carousel">
		<!--Carousel indicators-->
		<div
			class="absolute bottom-0 left-0 right-0 z-[2] mx-[15%] mb-4 flex list-none justify-center p-0"
			data-twe-carousel-indicators>
			<button
			type="button"
			data-twe-target="#carouselExampleCaptions"
			data-twe-slide-to="0"
			data-twe-carousel-active
			class="mx-[3px] box-content h-[3px] w-[30px] flex-initial cursor-pointer border-0 border-y-[10px] border-solid border-transparent bg-white bg-clip-padding p-0 -indent-[999px] opacity-50 transition-opacity duration-[600ms] ease-[cubic-bezier(0.25,0.1,0.25,1.0)] motion-reduce:transition-none"
			aria-current="true"
			aria-label="Slide 1"></button>
			<button
			type="button"
			data-twe-target="#carouselExampleCaptions"
			data-twe-slide-to="1"
			class="mx-[3px] box-content h-[3px] w-[30px] flex-initial cursor-pointer border-0 border-y-[10px] border-solid border-transparent bg-white bg-clip-padding p-0 -indent-[999px] opacity-50 transition-opacity duration-[600ms] ease-[cubic-bezier(0.25,0.1,0.25,1.0)] motion-reduce:transition-none"
			aria-label="Slide 2"></button>
			<button
			type="button"
			data-twe-target="#carouselExampleCaptions"
			data-twe-slide-to="2"
			class="mx-[3px] box-content h-[3px] w-[30px] flex-initial cursor-pointer border-0 border-y-[10px] border-solid border-transparent bg-white bg-clip-padding p-0 -indent-[999px] opacity-50 transition-opacity duration-[600ms] ease-[cubic-bezier(0.25,0.1,0.25,1.0)] motion-reduce:transition-none"
			aria-label="Slide 3"></button>
		</div>

		<!--Carousel items-->
		<div
			class="relative w-full h-[700px] overflow-hidden after:clear-both after:block after:content-['']">
			<!--First item-->
			<div
			class="relative float-left -mr-[100%] w-full transition-transform duration-[600ms] ease-in-out motion-reduce:transition-none"
			data-twe-carousel-active
			data-twe-carousel-item
			style="backface-visibility: hidden">
			<img
				:src="slide"
				class="block w-full object-cover"
				alt="..." />
			<div
				class="absolute inset-x-[15%] bottom-5 hidden py-5 text-center text-white md:block">
				<h5 class="text-3xl text-orange-900 font-bold [text-shadow:_0_1px_0_rgb(255_255_255_/_40%)]">Ginnidevi Satyanarayan Sekhsaria Girls' PG College</h5>
				<p class="font-bold">
				Affiliated to the PDU Shekhawati University, Sikar
				</p>
			</div>
			</div>
			<!--Second item-->
			<div
			class="relative float-left -mr-[100%] hidden w-full transition-transform duration-[600ms] ease-in-out motion-reduce:transition-none"
			data-twe-carousel-item
			style="backface-visibility: hidden">
			<img
				:src="slide2"
				class="block w-full"
				alt="..." />
			<div
				class="absolute inset-x-[15%] bottom-10 hidden py-5 text-center text-white md:block">
				<h5 class="text-3xl text-orange-900 font-bold [text-shadow:_0_1px_0_rgb(255_255_255_/_40%)]">Accredited B++ by NAAC</h5>
				
			</div>
			</div>
			<!--Third item-->
			<div
			class="relative float-left -mr-[100%] hidden w-full transition-transform duration-[600ms] ease-in-out motion-reduce:transition-none"
			data-twe-carousel-item
			style="backface-visibility: hidden">
			<img
				:src="slide3"
				class="block w-full"
				alt="..." />
			<div
				class="absolute inset-x-[15%] bottom-10 hidden py-5 text-center text-white md:block">
				<h5 class="text-3xl text-orange-900 font-bold [text-shadow:_0_1px_0_rgb(255_255_255_/_40%)]">Accredited B++ by NAAC</h5>
			</div>
			</div>
		</div>

		<!--Carousel controls - prev item-->
		<button
			class="absolute bottom-0 left-0 top-0 z-[1] flex w-[15%] items-center justify-center border-0 bg-none p-0 text-center text-white opacity-50 transition-opacity duration-150 ease-[cubic-bezier(0.25,0.1,0.25,1.0)] hover:text-white hover:no-underline hover:opacity-90 hover:outline-none focus:text-white focus:no-underline focus:opacity-90 focus:outline-none motion-reduce:transition-none"
			type="button"
			data-twe-target="#carouselExampleCaptions"
			data-twe-slide="prev">
			<span class="inline-block h-8 w-8">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				stroke-width="1.5"
				stroke="currentColor"
				class="h-6 w-6">
				<path
				stroke-linecap="round"
				stroke-linejoin="round"
				d="M15.75 19.5L8.25 12l7.5-7.5" />
			</svg>
			</span>
			<span
			class="!absolute !-m-px !h-px !w-px !overflow-hidden !whitespace-nowrap !border-0 !p-0 ![clip:rect(0,0,0,0)]"
			>Previous</span
			>
		</button>
		<!--Carousel controls - next item-->
		<button
			class="absolute bottom-0 right-0 top-0 z-[1] flex w-[15%] items-center justify-center border-0 bg-none p-0 text-center text-white opacity-50 transition-opacity duration-150 ease-[cubic-bezier(0.25,0.1,0.25,1.0)] hover:text-white hover:no-underline hover:opacity-90 hover:outline-none focus:text-white focus:no-underline focus:opacity-90 focus:outline-none motion-reduce:transition-none"
			type="button"
			data-twe-target="#carouselExampleCaptions"
			data-twe-slide="next">
			<span class="inline-block h-8 w-8">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				stroke-width="1.5"
				stroke="currentColor"
				class="h-6 w-6">
				<path
				stroke-linecap="round"
				stroke-linejoin="round"
				d="M8.25 4.5l7.5 7.5-7.5 7.5" />
			</svg>
			</span>
			<span
			class="!absolute !-m-px !h-px !w-px !overflow-hidden !whitespace-nowrap !border-0 !p-0 ![clip:rect(0,0,0,0)]"
			>Next</span
			>
		</button>
		</div>
	<Footer />
</template>

<route lang="yaml">
name: home
</route>
