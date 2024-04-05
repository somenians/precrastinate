<script lang="ts">
	import * as Dialog from '$lib/components/ui/dialog/index.js';
	import Label from '$lib/components/ui/label/label.svelte';
	import Button from '$lib/components/ui/button/button.svelte';
	import HamburgerMenu from 'svelte-radix/HamburgerMenu.svelte';

	let open = false;
</script>

<div>
	<Dialog.Root bind:open>
		<Dialog.Trigger asChild let:builder>
			<!-- <Button variant="outline" builders={[builder]}>Edit Profile</Button> -->
			<Button variant="ghost" size="icon" builders={[builder]}>
				<HamburgerMenu class="h-3 w-3" />
			</Button>
		</Dialog.Trigger>
		<Dialog.Content class="sm:max-w-[600px]">
			<Dialog.Header class="pb-8">
				<Dialog.Title>config</Dialog.Title>
				<Dialog.Description>--||WIP||--</Dialog.Description>
			</Dialog.Header>
			<form class="grid items-start gap-4">
				<div class="grid gap-2">
					<Label for="theme">theme</Label>
				</div>
				<Button variant="secondary" type="submit">save changes</Button>
			</form>
		</Dialog.Content>
	</Dialog.Root>
</div>
