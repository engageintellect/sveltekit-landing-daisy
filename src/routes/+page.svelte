<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import Carousel from '$lib/components/Carousel.svelte';
	import Chat from '$lib/components/Chat.svelte';
	import Countdown from '$lib/components/Countdown.svelte';
	import Drawer from '$lib/components/Drawer.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import Hero2 from '$lib/components/Hero2.svelte';
	import Hero3 from '$lib/components/Hero3.svelte';
	import Stats from '$lib/components/Stats.svelte';
</script>

<div>
	<div class="">
		<div class="">
			<Hero />
		</div>

		<div class="lg:container mx-auto">
			<Carousel />
		</div>
	</div>
	<div class="container mx-auto">
		<div class="p-4 xl:p-10 bg-base-300 my-10 rounded-lg">
			<div class="max-w-lg mx-auto">
				<div class="text-3xl font-bold text-center my-5">Instant Insights</div>
				<div class="text-lg text-center my-5">
					Voluptate eiusmod quis do aliquip labore esse pariatur excepteur dolore do fugiat sint
					Lorem commodo ea pariatur.
				</div>
			</div>
			<Stats />
		</div>

		<div class=" bg-base-300 p-4 xl:p-10 rounded-lg">
			<div class="max-w-lg mx-auto">
				<div class="text-3xl font-bold text-center my-5">Messages</div>
				<div class="text-lg text-center my-5">
					Voluptate eiusmod quis do aliquip labore esse pariatur excepteur dolore do fugiat sint
					officia. Commodo non est ullamco consectetur dolore excepteur.
				</div>
			</div>

			<Chat />
		</div>

		<div class="py-10">
			<Hero2 />
		</div>

		<div class="">
			<Hero3 />
		</div>
	</div>
</div>
