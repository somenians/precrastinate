<script>
	import '$lib/app.css';
	import Footer from '$lib/components/nav/Footer.svelte';
	import Header from '$lib/components/nav/Header.svelte';
</script>

<div class="min-h-screen relative">
	<Header />
	<div class="pb-8" />
	<slot />
	<Footer />
</div>
