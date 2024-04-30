<script context="module" lang="ts">
	const icons = [
		IconAccessibility,
		FluentEmojiArtistMediumDark,
		FluentEmojiEyes,
		FluentEmojiGrinningFaceWithSmilingEyes,
		IconAccountBox
	];
</script>

<script lang="ts">
	import IconAccessibility from '~icons/carbon/accessibility';
	import FluentEmojiArtistMediumDark from '~icons/fluent-emoji/artist-medium-dark';
	import FluentEmojiEyes from '~icons/fluent-emoji/eyes';
	import FluentEmojiGrinningFaceWithSmilingEyes from '~icons/fluent-emoji/grinning-face-with-smiling-eyes';
	import IconAccountBox from '~icons/mdi/account-box';

	import _ from 'lodash-es';

	const iconToRender = _.sample(icons);
</script>

<svelte:component this={iconToRender} />
