<script>
	import Icon from '$lib/components/Icon.svelte';
	import PngIcon from '$lib/components/PngIcon.svelte';
	import RenderDeepChild from '$lib/components/RenderDeepChild.svelte';
	import SvgIcon from '$lib/components/SvgIcon.svelte';
	import ToggleChildDisplay from '$lib/components/ToggleChildDisplay.svelte';
</script>

<main>
	<ToggleChildDisplay text="Direct Render">
		<Icon />
	</ToggleChildDisplay>

	<ToggleChildDisplay text="Direct Render Many Children">
		<Icon />
		<Icon />
		<Icon />
		<Icon />
		<Icon />
		<Icon />
		<Icon />
		<Icon />
		<Icon />
	</ToggleChildDisplay>

	<ToggleChildDisplay text="Direct Render PNG">
		<PngIcon />
	</ToggleChildDisplay>

	<ToggleChildDisplay text="Direct Render Many PNG">
		<PngIcon />
		<PngIcon />
		<PngIcon />
		<PngIcon />
		<PngIcon />
		<PngIcon />
		<PngIcon />
		<PngIcon />
		<PngIcon />
	</ToggleChildDisplay>

	<ToggleChildDisplay text="Direct Render SVG">
		<SvgIcon />
	</ToggleChildDisplay>

	<ToggleChildDisplay text="Direct Render Many SVG">
		<SvgIcon />
		<SvgIcon />
		<SvgIcon />
		<SvgIcon />
		<SvgIcon />
		<SvgIcon />
		<SvgIcon />
		<SvgIcon />
		<SvgIcon />
	</ToggleChildDisplay>

	<ToggleChildDisplay text="25 Deep Render">
		<RenderDeepChild depth={25}>
			<Icon />
		</RenderDeepChild>
	</ToggleChildDisplay>

	<ToggleChildDisplay text="25 Deep Render pure SVG">
		<RenderDeepChild depth={25}>
			<SvgIcon />
		</RenderDeepChild>
	</ToggleChildDisplay>

	<ToggleChildDisplay text="100 Deep Render">
		<RenderDeepChild depth={100}>
			<Icon />
		</RenderDeepChild>
	</ToggleChildDisplay>

	<ToggleChildDisplay text="100 Deep Render pure SVG">
		<RenderDeepChild depth={100}>
			<SvgIcon />
		</RenderDeepChild>
	</ToggleChildDisplay>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}
</style>
