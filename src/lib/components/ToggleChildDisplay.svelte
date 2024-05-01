<script lang="ts">
	import type { Snippet } from 'svelte';

	let showChild = $state(false);

	const { children, text }: { children: Snippet; text: string } = $props();
</script>

<button
	onclick={(e) => {
		console.trace('button onclick e: ', e);
		showChild = !showChild;
	}}
>
	{#if showChild}
		<!-- content here -->
		Hide
	{:else}
		Show
	{/if}
	{text}
</button>

{#if showChild}
	{@render children()}
{/if}
