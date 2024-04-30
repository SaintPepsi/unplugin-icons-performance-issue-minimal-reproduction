<script lang="ts">
	import type { Snippet } from 'svelte';
	const { depth, children }: { depth: number; children: Snippet } = $props();

	const renderWrapper = Math.random() > 0.5;
</script>

{#snippet content()}
	{#if depth > 0}
		<svelte:self depth={depth - 1}>
			{@render children()}
		</svelte:self>
	{:else}
		<div class="RenderedDeepChild">
			{@render children()}
		</div>
	{/if}
{/snippet}

{#if renderWrapper}
	<div class="RenderedDeepChild">
		{@render content()}
	</div>
	<!-- content here -->
{:else}
	{@render content()}
{/if}
