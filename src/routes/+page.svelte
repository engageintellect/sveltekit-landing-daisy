<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import Carousel from '$lib/components/Carousel.svelte';
	import Chat from '$lib/components/Chat.svelte';
	import Countdown from '$lib/components/Countdown.svelte';
	import Drawer from '$lib/components/Drawer.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import Hero2 from '$lib/components/Hero2.svelte';
	import Hero3 from '$lib/components/Hero3.svelte';
	import Hero4 from '$lib/components/Hero4.svelte';
	import Mobile from '$lib/components/Mobile.svelte';
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
		<Stats />
		<Chat />

		<div class="my-10">
			<Hero2 />
		</div>

		<div class="my-10">
			<Hero3 />
		</div>

		<div class="my-10">
			<Hero4 />
		</div>

		<div class="my-10">
			<Mobile />
		</div>
	</div>
</div>
