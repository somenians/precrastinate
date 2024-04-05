<script>
	import '$lib/app.css';
	import { HamburgerMenu } from 'svelte-radix';
	import Button from '../ui/button/button.svelte';
	import { onMount } from 'svelte';
	import Config from '../dialog/Config.svelte';
	import LogIn from '../dialog/LogIn.svelte';
</script>

<header class="lg:px-8 fixed w-full backdrop-blur-sm">
	<nav>
		<div class="flex flex-nowrap flex-row justify-around h-24 items-center">
			<a href="/">precrastinate</a>
			<div class="flex flex-row mx-8 space-x-6">
				<a href="/dashboard">dashboard</a>
				<a href="/todo">todo</a>
				<a href="/focus">focus</a>
			</div>
			<div class="flex flex-row items-center">
				<LogIn />
				<Config />
			</div>
		</div>
	</nav>
</header>
