<script lang="ts">
	import '$lib/app.css';
	import Button from '$lib/components/ui/button/button.svelte';
</script>

<div
	class="flex flex-col h-screen mx-auto max
    -w-screen-xl items-center justify-center lg:py-16 lg:px-12"
>
	<h1 class="mb-6 text-5xl md:text-6xl lg:text-8xl">precrastinate</h1>
	<p class="mb-10 text-l lg:text-2xl sm:px-16 xl:px-48">
		a simple app to help procrastinators alike stay on task
	</p>
	<Button variant="secondary" href="/todo">get started</Button>
</div>
