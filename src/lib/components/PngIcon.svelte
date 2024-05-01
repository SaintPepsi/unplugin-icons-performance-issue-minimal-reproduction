<script context="module" lang="ts">
	const icons = [
		IconAccessibility,
		FluentEmojiArtistMedium,
		FluentEmojiEyes,
		FluentEmojiGrinningFaceWithSmilingEyes,
		IconAccountBox
	];
</script>

<script lang="ts">
	import IconAccessibility from '$lib/images/carbon:accessibility.png';
	import FluentEmojiEyes from '$lib/images/fluent-emoji:eyes.png';
	import FluentEmojiGrinningFaceWithSmilingEyes from '$lib/images/fluent-emoji:grinning-face-with-smiling-eyes.png';
	import FluentEmojiArtistMedium from '$lib/images/fluent-emoji:man-cook-medium.png';
	import IconAccountBox from '$lib/images/mdi:account-box.png';
	import sample from 'lodash-es/sample';

	const iconToRender = sample(icons);
</script>

<img width="25" height="25" src={iconToRender} alt="png icon" />
