<script setup>
	import maa from '@/assets/maa-gss.jpg';
	import slide from '@/assets/gss-slide.jpg';
	useHead({
		title: 'GSS Girls PG College, Chirawa',
	});
</script>

<template>
	<AppHeader />
	<div
		class="relative h-[400px] overflow-hidden bg-[url('gss-slide.jpg')] bg-cover bg-no-repeat p-12 text-center text-white">
		<div
			class="absolute bottom-0 left-0 right-0 top-0 h-full w-full overflow-hidden bg-black/30 bg-fixed">
			<div class="flex h-full items-end justify-center">
			<div class="text-white">
				<h2 class="mb-4 text-4xl font-semibold">GinniDevi Satyanarayan Shekhsaria Girls' PG College</h2>
				<h4 class="mb-6 text-xl font-semibold">Accredited B++ by NAAC</h4>
				<h4 class="mb-6 text-xl font-semibold">Affiliated to PDU Shekhawati University, Sikar</h4>
			</div>
			</div>
		</div>
	</div>
	<Footer />
</template>

<route lang="yaml">
name: home
</route>
