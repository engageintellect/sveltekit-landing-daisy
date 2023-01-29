<script lang="ts">
	import { enhance, type SubmitFunction } from '$app/forms';
	import { page } from '$app/stores';
	import '$lib/app.css';
	import Nav from '$lib/components/Nav.svelte';
</script>

<div class="bg-base-200">
	<Nav />

	<div class="">
		<slot />
	</div>
</div>
