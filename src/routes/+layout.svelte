<script lang="ts">
	import '$lib/app.css';
	import Nav from '$lib/components/Nav.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<div class="bg-base-200">
	<Nav />

	<div class="">
		<slot />
	</div>
	<Footer />
</div>
