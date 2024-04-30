<script lang="ts">
	import type { Snippet } from 'svelte';
	import SvgSpinners8DotsRotate from '~icons/svg-spinners/8-dots-rotate';
	const { children }: { children: Snippet } = $props();
</script>

<SvgSpinners8DotsRotate />

{@render children()}
