<script lang="ts">
	import { enhance, type SubmitFunction } from '$app/forms';
	import { page } from '$app/stores';
	import '$lib/app.css';
	import Drawer from './Drawer.svelte';

	const submitUpdateTheme: SubmitFunction = ({ action }) => {
		const theme = action.searchParams.get('theme');

		if (theme) {
			document.documentElement.setAttribute('data-theme', theme);
		}
	};

	const themes = [
		'light',
		'dark',
		'cupcake',
		'bumblebee',
		'emerald',
		'corporate',
		'synthwave',
		'retro',
		'cyberpunk',
		'valentine',
		'halloween',
		'garden',
		'forest',
		'aqua',
		'lofi',
		'pastel',
		'fantasy',
		'wireframe',
		'black',
		'luxury',
		'dracula',
		'cmyk',
		'autumn',
		'business',
		'acid',
		'lemonade',
		'night',
		'coffee',
		'winter'
	];
</script>

<div class="bg-base-100 sticky top-0 shadow-lg z-40">
	<div class="flex items-center justify-between p-2 lg:container lg:mx-auto">
		<div class="">
			<a href="/" class="font-bold text-primary text-xl">Sveltekit</a>
		</div>

		<div class="">
			<div class="dropdown dropdown-hover dropdown-end">
				<!-- svelte-ignore a11y-label-has-associated-control -->
				<label class="btn">Theme</label>
				<!-- svelte-ignore a11y-no-noninteractive-tabindex -->
				<ul tabindex="0" class="dropdown-content menu p-2 shadow bg-base-100 h-96 overflow-scroll">
					<form method="POST" use:enhance={submitUpdateTheme}>
						{#each themes as theme}
							<li>
								<button formaction="/?/setTheme&theme={theme}&redirectTo={$page.url.pathname}"
									>{theme}</button
								>
							</li>
						{/each}
					</form>
				</ul>
			</div>
		</div>
	</div>
</div>
