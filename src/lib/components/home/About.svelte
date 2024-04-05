<script lang="ts">
	import '$lib/app.css';
	import Features from './features/Features.svelte';
</script>

<div class="flex flex-wrap flex-row justify-around items-center h-screen mb-16 lg:py-16 lg:px-16">
	<!-- flex flex-nowrap flex-row justify-around h-24 items-center -->
	<div class="flex flex-col max-w-xl">
		<h1 class="mb-6 text-xl md:text-3xl lg:text-6xl">why precrastinate?</h1>
		<p class="mb-16 pr-21 text-l lg:text-2xl">
			its hard to get work done. because of that, you should try out some of our features.
		</p>
	</div>
	<Features />
	<!-- <p class="mb-10 font-extrabold text-l lg:text-2xl">we have:</p> -->
</div>
